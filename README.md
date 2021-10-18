# tfe-validcertificate-vagrant
Install TFE on Demo version with Valid Certificate - vagrant. How : TFE auto install in local VM with valid certificate.
## Pre-requirements

## Pre-requirements

* [Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) 
* [Vagrant](https://www.vagrantup.com/docs/installation)
* [VirtualBox](https://www.virtualbox.org/wiki/Downloads)


## How to use this repo

- Clone
- Run
- Cleanup

---

### Clone the repo

```
git clone https://github.com/ayahmuhamed/tfe-validcertificate-vagrant
```

### Change directory

```
cd tfe-validcertificate-vagrant
```

### Run

* Copy your license file to config/license.rli (for TF Support Engineer, check 1Password Support Engineering Vault, hashicorp-internall---support.rli)

```
cp /path/to/your/license config/license.rli
```

_sample_ :

```
cp ~/Downloads/hashicorp-internal---support.rli config/license.rli
```

* Bring up the VMs:

```
vagrant up
```


* TFE components need some time for first initialization. You may poll the _/_health_check_ endpoint until a _200_ is returned by the application, indicating that it is fully started:


```




* Enter *Password!* to unlock the console

```


### Cleanup

```
vagrant destroy -f
```

