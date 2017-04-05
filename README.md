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
updeployment_rsync_src: "localhost"
updeployment_rsync_extra_params: ""

# Path where the code must be deployed to
updeployment_deploy_to: "/var/www/my-app"

# Folder name for the releases
updeployment_version_dir: "releases"

# Softlink name for the current release
updeployment_current_dir: "current"

# Current directory deployment strategy
updeployment_current_via: "symlink"

# Number of releases to keep in your hosts, if 0, unlimited releases will be kept
updeployment_keep_releases: 0
```