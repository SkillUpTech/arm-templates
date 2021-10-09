# Azure Resource Manager (ARM) Templates

This repository hosts useful ARM templates at public URLs (https://raw.githubusercontent.com/SkillUpTech/arm-templates/main/...).

## Available Templates

Simply click one of the buttons below to perform a deployment. For more information about a particular template, see the `README.md` file in the corresponding subdirectory.

### focal-py38-docker
[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FSkillUpTech%2Farm-templates%2Fmain%2Ffocal-py38-docker%2Fazuredeploy.json)

Ubuntu 20.04 Server VM with Docker, Docker Compose, and Python 3.8 pre-installed. 
- Uses a `D2as_v4` VM by default.
- A data disk is added and mounted to `/storage` (defaults to 64GiB).
- A restart will occur shortly after the deployment succeeds.
    - Please allow some time for this to occur.
    - Once this reboot completes, Docker will become available.

### focal-openedx-tutor
[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FSkillUpTech%2Farm-templates%2Fmain%2Ffocal-openedx-tutor%2Fazuredeploy.json)

The same as `focal-py38-docker` but with some Python modules for OpenEdx development preinstalled.
