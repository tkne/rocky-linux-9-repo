Rocky Linux 9 (Blue Onyx) yum repository
======

Working Rocky Linux 9 yum repository files to replace the .repo files in your /etc/yum.repos.d folder on your Rocky Linux 9 server.

## Usage:
Navigate to the `/etc` folder:
```bash
cd /etc
```

</br>

Backup your current `yum.repos.d` folder first:
```bash
mv yum.repos.d yum.repos.d_old
```

</br>

Clone the new `yum.repos.d` folder to your system:
```bash
git clone https://github.com/tkne/rocky-linux-9-repo.git yum.repos.d
```

</br>

Clean the local cache:
```bash
dnf clean all
```

</br>

Update the installed packages on your system:
```bash
dnf update
```

</br>

In case you have other external repositories installed as well, you'll need to edit each .repo dotfile and replace the settings manually.