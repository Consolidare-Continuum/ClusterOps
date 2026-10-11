# CC adapt — ClusterOps

**Package:** `clusterops` **0.3.0+cc0** (MIT; PEP 440 local label for wave tag `0.3.0cc0`)  
**Repo:** https://github.com/Consolidare-Continuum/ClusterOps  
**Parent:** fork of The-Swarm-Corporation/ClusterOps (Swarms)

## Dual vestment

| Vestment | Where | Role |
|----------|-------|------|
| **Brain shim** | `CC_.com/scripts/clusterops` + `requirements-clusterops-shim.txt` | Interim CPU affinity for heavy jobs (`PYTHONPATH=scripts`) |
| **CC package** | this repo | Prefer when editable/released; same CPU surface, no Ray required |

GPU helpers stay behind extras — do not pull Ray into CPU-only job venvs.

## Install

```bash
# CPU-only (default)
pip install -e .
# or: pip install -r requirements.txt && pip install -e .

# GPU (Ray + GPUtil)
pip install -e '.[gpu]'
# or: pip install -r requirements-gpu.txt
```

## Brain pointers

- Spec: `governance/SPEC-ETHAN-CLUSTEROPS-BRAIN-WIDE.md`
- Shim README: `scripts/clusterops/README.md`
- Abelard venv note: `operational/assignments/reports/COPS-020-ALTITUDINE-VENV.md`

SIGNED: Developer (Felix) | Claude Code context | 2026-09-08 | COPS-037..042 packaging
