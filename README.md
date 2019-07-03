# Ansible Role - Helm

Role to install, configure and start Helm

## Configure Versions

Use the following variables to customise the versions installed:

```
helm_version: v2.8.2
helm_platform: linux-amd64
helm_mirror: https://storage.googleapis.com/kubernetes-helm
```

## Helm Repos

To add helm repositories list them under the `helm_repos` variable:

```
helm_repos:
  - name: myrepo
    url: http://myrepo.com:8888
  - name: myotherrepo
    url: http://myotherrepo.com:8888
```

This role will add the repos, so any existing (if helm is already installed) will remain
