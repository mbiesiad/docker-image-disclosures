# Pagekit Docker Image Exposes .htaccess File

# Description
The community Pagekit Docker image (pagekit/pagekit on Docker Hub) allows public access to the .htaccess file located in the web root. 
This file contains configuration rules for Apache and should not be exposed, as it can reveal sensitive application details and URL rewrites. 
The exposure is due to a missing Apache configuration directive to deny access to hidden files (e.g., <Files ".ht*"> Require all denied </Files>).

# Proof of Concept
Screenshot

<img width="1147" height="358" alt="poc-pagekit-htaccess" src="https://github.com/user-attachments/assets/1247c46e-6fca-4157-ae49-5bfeb390fe4a" />


# Details
- Affected Docker image: `pagekit/pagekit`

- Affected Docker image - link: https://hub.docker.com/r/pagekit/pagekit

- Docker image description: 
"Ubuntu + Nginx + PHP5-fpm + Pagekit CMS + MySQL or SQLite"

- Type: Community

- Updated: over 7 years ago 

- Disclosure date: 2025-11-30

Discovered by mbiesiad

CWE:
- CWE-200: Exposure of Sensitive Information to an Unauthorized Actor
- CWE-284: Improper Access Control
- CWE-285: Improper Authorization

References
- https://github.com/izuolan/dockerfiles/tree/master/pagekit
- https://www.acunetix.com/vulnerabilities/web/htaccess-file-detected/
- https://www.invicti.com/web-vulnerability-scanner/vulnerabilities/htaccess-file-detected
- https://github.com/izuolan/dockerfiles/issues/6
