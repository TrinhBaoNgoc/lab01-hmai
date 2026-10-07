# Study Assistant — starter

A starter repository for the CSC10014 Smart Virtual Assistant project.

## Setup
Prerequisites: Python 3.10+, Git.

```bash
  git clone [https://github.com/TrinhBaoNgoc/lab01-hmai.git](https://github.com/TrinhBaoNgoc/lab01-hmai.git)
  cd lab01-hmai 
  python -m venv .venv 
  source .venv/Scripts/activate            # Windows: .venv\Scripts\Activate.ps1 
  
  # UPDATE PIP IF USING AN OLDER VERSION:
  python -m pip install --upgrade pip
  
  pip install -r requirements.txt  
  pip install -e .
```
## Run
```bash
   python -m assistant "where is the library?"
```
  -> Library: room B.201, open Mon-Sat 07:00-20:00. 

## Test

```bash
  pytest -q
```

## Project structure

- "No module named assistant" -> you forgot `pip install -e .` or the venv is not active. 
- PowerShell blocks Activate.ps1 -> Set-ExecutionPolicy -Scope CurrentUser RemoteSigned 

## Troubleshooting

If a package is missing, outdated, or installed with the wrong version:

1. **Ensure your virtual environment is active:**
   - Linux / macOS / Git Bash:
     ```bash
     source .venv/Scripts/activate
     ```
   - Windows PowerShell:
     ```powershell
     .venv\Scripts\Activate.ps1
     ```

2. **Re-sync pinned packages with `requirements.txt`:**
   Force pip to reinstall the exact pinned versions specified in the repository:
   ```bash
   pip install --force-reinstall -r requirements.txt
