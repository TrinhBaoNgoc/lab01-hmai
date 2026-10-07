# Lab 1 homework — Break your setup, recover from the README


| What I broke | Error message I saw | How I fixed it | README change needed? |
|---|---|---|---|
| Deleted the `.venv` virtual environment folder (`rm -rf .venv`). | `pytest: command not found`<br> | Followed the exact steps in `README.md`:<br>1. Re-created venv: `python -m venv .venv`<br>2. Activated venv: `source .venv/Scripts/activate` <br>3. Upgraded pip: `python -m pip install --upgrade pip`<br>4. Installed pinned dependencies: `pip install -r requirements.txt`<br>5. Installed editable package: `pip install -e .` | Yes. Added guidance for re-create .venv in Troubleshooting |

Commit the README fix (if any) with a Conventional Commit message:
----
- **Commit hash/message:** `docs: fix wrong link github`
- **Commit URL:** `https://github.com/TrinhBaoNgoc/lab01-hmai/commit/5ac30d9`
----
- **Commit hash/message:** docs: revise README with setup and troubleshooting details.  
- **Commit URL:** `https://github.com/TrinhBaoNgoc/lab01-hmai/commit/f7ccdee`
----
- **Commit hash/message:** docs: Fix troubleshooting steps in README
- **Commit URL:** `https://github.com/TrinhBaoNgoc/lab01-hmai/commit/9086216`