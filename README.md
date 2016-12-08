### UPYUN Node.js Application version control utility (Deploy)

folk from ansistrano-deployment

for internal used.

## usage

```yaml
# 获取源码到 project 目录
- git:
    src:
    dest:

- roles:
  - upyun-dev.deploy
```

## variables

```yml
ansistrano_rsync_src: "localhost"
ansistrano_rsync_extra_params: ""

# Path where the code must be deployed to
ansistrano_deploy_to: "/var/www/my-app"

# Folder name for the releases
ansistrano_version_dir: "releases"

# Softlink name for the current release
ansistrano_current_dir: "current"

# Current directory deployment strategy
ansistrano_current_via: "symlink"

# Number of releases to keep in your hosts, if 0, unlimited releases will be kept
ansistrano_keep_releases: 0
```