# focal-py38-docker

*Development VM for the OpenEdx Platform via Tutor*

Azure Resource Manager (ARM) template for an OpenEdx development VM with Docker, Docker Compose, Python3.8, `tutor`, and the `tutor-recon` plugin pre-installed.

This template effectively uses `focal-py38-docker` as a "parent template". 
- It defines a single resource (the parent deployment). 
- The only true difference is that this template will find its own `cloud-config.yaml` file. 
    - The file starts by simply `#include`ing the `cloud-config.yaml` file from the parent template.
    - Then, a couple of additional modules are added for Tutor... and that's it!
