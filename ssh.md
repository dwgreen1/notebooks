ssh Quick Start
=========

* What is ssh?

* Generate Keys

```bash
ssh-keygen -t rsa -b 4096 -f <name of keypair>
```

* Generate keys on local system, if you haven't already
* Add your key(s) to your local system (ssh-add …)
  * `ssh-add -K ~/.ssh/id_rsa.pub`
* Copy to the remote server:
  * `ssh-copy-id -i ~/.ssh/id_rsa.pub me@email.com`
