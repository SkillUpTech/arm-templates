# Azure Resource Manager (ARM) Templates

This repository hosts useful ARM templates at public URLs (https://raw.githubusercontent.com/SkillUpTech/arm-templates/main/...).

## Available Templates

### focal-py38-docker
[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FSkillUpTech%2Farm-templates%2Fmain%2Ffocal-py38-docker%2Fazuredeploy.json)

Ubuntu 20.04 Pro development VM with Docker and Python 3.8 pre-installed. 
- Uses a `D2as_v4` VM by default.
- A data disk is added and mounted to `/storage` (defaults to 64GiB).
- A restart will occur shortly after the deployment succeeds.
    - Please allow some time for this to occur.
    - Once this reboot completes, docker will become available.
