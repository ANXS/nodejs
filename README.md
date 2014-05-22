## Ansibles - nodejs [![Build Status](https://travis-ci.org/mtpereira/nodejs.svg)](https://travis-ci.org/mtpereira/nodejs)

Ansible role for installing nodejs, from package or by building it from source.


#### Requirements & Dependencies
- Tested on Ansible 1.4 or higher.
- Depends on Ansibles.build-essential


#### Variables

```yaml
nodejs_install_method: "source"     # "package" or "source"
nodejs_version: "0.10.26"           # nodejs version to install.
```


#### License

Licensed under the MIT License. See the LICENSE file for details.


#### Feedback, bug-reports, requests, ...

Are [welcome](https://github.com/ansibles/nodejs/issues)!
