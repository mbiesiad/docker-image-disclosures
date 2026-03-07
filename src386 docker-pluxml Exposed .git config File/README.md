# src386/docker-pluxml Docker Image Exposes .git/config File

# Description
The Git configuration file is publicly accessible via HTTP. 
The `.git/config` file contains repository configuration including remote repository URLs and other metadata. While not always highly sensitive by itself, its exposure confirms that the `.git` directory is accessible and may allow further repository enumeration.

# Proof of Concept
Screenshot

<img width="588" height="164" alt="poc-dockerImage-pluxml-exposed-git-config" src="https://github.com/user-attachments/assets/0e861cb1-d186-45a8-99a5-9d8849447ac0" />

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
