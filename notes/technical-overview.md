---
slug: github-8rivers-note-technical-overview
id: github-8rivers-note-technical-overview
title: 8rivers Overview
repo: justin-napolitano/8rivers
githubUrl: https://github.com/justin-napolitano/8rivers
generatedAt: '2025-11-24T18:30:00.306Z'
source: github-auto
summary: >-
  8rivers is a toolkit for automating the build, deployment, and backup of web
  documentation projects. It leverages Python and shell scripting for tasks like
  dependency management, HTML documentation generation, and cloud backups.
tags: []
seoPrimaryKeyword: ''
seoSecondaryKeywords: []
seoOptimized: false
topicFamily: null
topicFamilyConfidence: null
kind: note
entryLayout: note
showInProjects: false
showInNotes: true
showInWriting: false
showInLogs: false
---

8rivers is a toolkit for automating the build, deployment, and backup of web documentation projects. It leverages Python and shell scripting for tasks like dependency management, HTML documentation generation, and cloud backups.

## Key Features

- Install Python dependencies using pip
- Generate HTML docs with Makefile and Sphinx
- Deploy to GitHub Pages via GitHub CLI
- Backup to Dropbox with the Dropbox API

## Getting Started

### Prerequisites

- Python 3.5+
- pip
- Dropbox API token
- GitHub CLI

### Quick Setup

Clone the repo and install dependencies:

```bash
git clone https://github.com/justin-napolitano/8rivers.git
cd 8rivers
pip install -r requirements.txt
```

### Run Commands

Build the documentation:

```bash
make html
```

Deploy to GitHub Pages:

```bash
./deploy.sh
```

Backup to Dropbox:

```bash
python3 backup_html.py
```

### Gotchas

Ensure your Dropbox token is set in `backup_html.py`. Check for duplicate requirements with `requirements.txt` and `requirments.txt`.
