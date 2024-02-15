Rocky Linux 9 (Blue Onyx) yum repository
======

Working Rocky Linux 9 yum repository files to replace the files in your /etc/yum.repos.d folder on your Rocky Linux 9 server.

In a vanilla setup use the following:
```bash
cd /etc
mv yum.repos.d yum.repos.d_old
git clone https://github.com/tkne/rocky-linux-9-repo.git yum.repos.d
dnf clean all
dnf update
```

In case you have other external repositories installed as well, you'll need to edit each repository dotfile and replace the settings by hand.