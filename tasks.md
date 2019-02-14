Tasks
=====
A collection commands for tasks that I've needed to perform multiple times.

## Delete Old Kernels, Classic Version

```bash
uname -r # the kernel in use
```

```bash
dpkg -l | grep linux-image | awk '{print$2}'
```

```bash
apt remove --purge linux-image-3.1.0-131-generic
```

```bash
update-grub
```

## Find the Size of a Directory

```bash
du -hs /path/to/directory
```