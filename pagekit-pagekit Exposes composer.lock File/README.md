# Pagekit Docker Image Exposes composer.lock File

# Description
The community Pagekit Docker image (pagekit/pagekit on Docker Hub) allows public access to the `composer.lock` file located in the web root. 

# Proof of Concept
Screenshot

<img width="640" height="110" alt="poc-dockerImage-pageKit-composerLock" src="https://github.com/user-attachments/assets/4a2b10bf-ef8a-4cb4-a7e8-32e7dad349e5" />

# Details
- Affected Docker image: `pagekit/pagekit`

- Affected Docker image - link: https://hub.docker.com/r/pagekit/pagekit

- Docker image description: 
"Ubuntu + Nginx + PHP5-fpm + Pagekit CMS + MySQL or SQLite"

- Type: Community

- Downloads: 10K+

- Updated: over 7 years ago 

- Disclosure date: 2025-12-01

Discovered by mbiesiad

CWE:
- CWE-200: Exposure of Sensitive Information to an Unauthorized Actor
- CWE-284: Improper Access Control
- CWE-285: Improper Authorization
- CWE-538: Insertion of Sensitive Information into Externally-Accessible File or Directory

References
- https://github.com/izuolan/dockerfiles/tree/master/pagekit
- https://github.com/izuolan/dockerfiles/issues/7
- https://hub.docker.com/r/pagekit/pagekit 

## Disclaimer
For educational and defensive purposes only. 
