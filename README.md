## ANXS - nodejs [![Build Status](https://travis-ci.org/ANXS/nodejs.png)](https://travis-ci.org/ANXS/nodejs)

Ansible role for installing nodejs, from package or by building it from source.


#### Requirements & Dependencies
- Tested on Ansible 1.4 or higher.
- Depends on ANXS.build-essential when using install_method of "source"

#### Variables

```yaml
nodejs_version: "0.10.26"           # nodejs version to install.
nodejs_install_method: "source"     # "package" or "source" or "binary"
```

For "unstable" node versions (0.11), you may wish to use "binary" if you don't want to compile from source:

```yaml
nodejs_version: "0.11.13"           # nodejs version to install.
nodejs_install_method: "binary"     # "source" or "binary" (package is not available for 0.11)
```

#### Thanks to
- [Nicolas Bazire](https://github.com/nicbaz)
- [Luís Couto](https://github.com/Couto)
- [Stephan Hochhaus](https://github.com/yauh)
- [Nathan Palmer](https://github.com/nathanpalmer)
- [Manuel Tiago Pereira](https://github.com/mtpereira)
- [Umair Siddique](https://github.com/umairsiddique)


#### Testing
This project comes with a VagrantFile, this is a fast and easy way to test changes to the role, fire it up with `vagrant up`

See [vagrant docs](https://docs.vagrantup.com/v2/) for getting setup with vagrant


#### License

Licensed under the MIT License. See the LICENSE file for details.


#### Feedback, bug-reports, requests, ...

Are [welcome](https://github.com/ANXS/nodejs/issues)!
