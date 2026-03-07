# src386/docker-pluxml Docker Image Exposes .git/index File

# Description
The Git index file is accessible via HTTP.
The `.git/index` file contains a list of files tracked by the repository and metadata about them. This file can be used together with other `.git` data to reconstruct the repository contents.

# Proof of Concept
Screenshot

<img width="1034" height="316" alt="poc-dockerImage-pluxml-exposed-git-index" src="https://github.com/user-attachments/assets/d5c07214-d957-450e-966e-87c75385246b" />

# Details
- Affected Docker image: https://github.com/src386/docker-pluxml/tree/master/5.8 
- Dockerfile: pluxml__version=v5.8.9
- Disclosure date: 2026-03-07

Discovered by mbiesiad

CWE:
- CWE-200: Exposure of Sensitive Information to an Unauthorized Actor
- CWE-284: Improper Access Control
- CWE-552: Files or Directories Accessible to External Parties

References
- https://github.com/src386/docker-pluxml 
- https://github.com/src386/docker-pluxml/tree/master/5.8

## Disclaimer
For educational and defensive purposes only.
