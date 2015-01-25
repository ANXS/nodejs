## ANXS - nodejs [![Build Status](https://travis-ci.org/ANXS/nodejs.png)](https://travis-ci.org/ANXS/nodejs)

Ansible role for installing nodejs, from package or by building it from source.


#### Requirements & Dependencies
- Tested on Ansible 1.4 or higher.
- Depends on ANXS.build-essential


#### Variables

```yaml
nodejs_install_method: "source"     # "package" or "source"
nodejs_version: "0.10.26"           # nodejs version to install.
```

#### Thanks to
- [Nicolas Bazire](https://github.com/nicbaz)
- [Luís Couto](https://github.com/Couto)
- [Stephan Hochhaus](https://github.com/yauh)
- [Nathan Palmer](https://github.com/nathanpalmer)
- [Manuel Tiago Pereira](https://github.com/mtpereira)
- [Umair Siddique](https://github.com/umairsiddique)


#### License

Licensed under the MIT License. See the LICENSE file for details.


#### Feedback, bug-reports, requests, ...

Are [welcome](https://github.com/ANXS/nodejs/issues)!
