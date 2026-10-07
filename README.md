# Study Assistant — starter

A starter repository for the CSC10014 Smart Virtual Assistant project.

## Setup
Prerequisites: Python 3.10+, Git. 
  
    git clone git@github.com:<you>/lab01-hmai.git 
    cd lab01-hmai 
    python -m venv .venv 
    source .venv/bin/activate            # Windows: .venv\Scripts\Activate.ps1 
    pip install -r requirements.txt 
    pip install -e .
## Run

   python -m assistant "where is the library?" 
    # -> Library: room B.201, open Mon-Sat 07:00-20:00. 

## Test

pytest -q

## Project structure

- "No module named assistant" -> you forgot `pip install -e .` or the venv is not active. 
- PowerShell blocks Activate.ps1 -> Set-ExecutionPolicy -Scope CurrentUser RemoteSigned 
