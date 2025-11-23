# 8rivers

A versatile collection of scripts and tools primarily focused on building, deploying, and backing up web documentation and projects. This repository includes automation for dependency management, HTML build processes, Dropbox backup integration, and deployment workflows.

## Features

- Automated dependency installation via pip
- HTML documentation build and deployment using Makefile and GitHub Pages
- Backup of build artifacts to Dropbox using their API
- Various shell scripts for setup, deployment, and maintenance tasks
- Dockerfile for containerized environments

## Tech Stack

- Python (3.5+)
- Bash scripting
- Makefile
- Dropbox API
- Docker
- Sphinx documentation builder

## Getting Started

### Prerequisites

- Python 3.5 or higher
- pip
- Dropbox API token (for backup scripts)
- Make
- GitHub CLI (for deployment script `deploy.sh`)

### Installation

Clone the repository:

```bash
git clone https://github.com/justin-napolitano/8rivers.git
cd 8rivers
```

Install Python dependencies:

```bash
pip install -r requirements.txt
```

### Usage

Build the HTML documentation:

```bash
make html
```

Deploy the built documentation to GitHub Pages:

```bash
./deploy.sh
```

Backup the built HTML to Dropbox (ensure you have set your access token in `backup_html.py`):

```bash
python3 backup_html.py
```

Run setup scripts or other utilities as needed, for example:

```bash
./install.sh
./uninstall.sh
```

## Project Structure

```
8rivers/
├── acp.sh                # Shell script (purpose assumed for automation)
├── backup_html.py        # Python script to backup build/html to Dropbox
├── chtml.sh              # Shell script (likely related to HTML build)
├── deploy.sh             # Deploy built docs to GitHub Pages
├── deployz.sh            # Another deployment script variant
├── Dockerfile            # Docker container setup
├── doit.sh               # Shell script (task automation)
├── install.sh            # Setup script
├── label_list.py         # Python script to read and print label data from pickle files
├── latex/                # Directory likely containing LaTeX templates or sources
├── LICENSE               # License file
├── mac_setup.sh          # Mac-specific setup script
├── Makefile              # Build automation for docs and other tasks
├── overview.rst          # ReStructuredText overview document
├── pullit.sh             # Shell script to pull updates
├── pushit.sh             # Shell script to push updates
├── python_build.py       # Python script automating build pipeline
├── README.md             # This file
├── requirements.txt      # Python dependencies
├── requirments.txt       # Possibly duplicate or typo for requirements
├── res.text              # Resource text file
├── source/               # Source files for documentation
├── test.text             # Test text file
└── uninstall.sh          # Uninstall script
```

## Future Work / Roadmap

- Improve documentation and add detailed usage instructions
- Consolidate and clean up duplicate files like `requirements.txt` and `requirments.txt`
- Add unit tests for Python scripts
- Enhance Dropbox backup script to support folder uploads and error handling
- Containerize the entire build and deployment pipeline via Docker
- Add CI/CD integration for automated builds and deployments
- Expand README with examples and troubleshooting tips

---

*Note: Some assumptions were made about the purpose of scripts and files based on their names and partial contents.*