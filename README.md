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
deploy_rsync_src: "localhost"
deploy_rsync_extra_params: ""

# Path where the code must be deployed to
deploy_to: "/var/www/my-app"

# Folder name for the releases
deploy_version_dir: "releases"

# Softlink name for the current release
deploy_current_dir: "current"

# Current directory deployment strategy
deploy_current_via: "symlink"

# Number of releases to keep in your hosts, if 0, unlimited releases will be kept
deploy_keep_releases: 0
```