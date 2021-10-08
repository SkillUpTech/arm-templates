This directory contains cloud-config modules for adding features to VMs.

### Assumptions

All templates assume that the admin user is named `vm-root`.

### Samples

Sample `cloud-config.yaml` file which includes some modules from this directory:

```
#include
https://raw.githubusercontent.com/SkillUpTech/arm-templates/main/common/cloud-init/focal/base.yaml
https://raw.githubusercontent.com/SkillUpTech/arm-templates/main/common/cloud-init/focal/python38.yaml
```

A VM provided with this userdata will: 

- Add some useful base packages.
- Install python3.8.
