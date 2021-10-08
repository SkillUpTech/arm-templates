This directory contains cloud-config modules for adding features to VMs.

### Assumptions

All templates assume that the admin user is named `vm-root`.

### Samples

Sample `cloud-config.yaml` file which includes some modules from this directory:

```yaml
#cloud-config
merge_how:
 - name: list
   settings: [append]
 - name: dict
   settings: [no_replace, recurse_list]

#include
https://raw.githubusercontent.com/SkillUpTech/arm-templates/main/common/cloud-init/focal/base.yaml
https://raw.githubusercontent.com/SkillUpTech/arm-templates/main/common/cloud-init/focal/python38.yaml
```

A VM with this userdata will add 

- Add some useful base packages.
- Install python3.8.

Note the `merge_how` key--without this configuration, each module will supplant the settings given in the previous one (bad!). These modules expect to be combined with other modules as needed, so make sure to add the `merge_how` configuration prior to `#include`ing modules from this directory.
