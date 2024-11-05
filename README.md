# Config Repo

This repo is the source of my CircleCI config. This is the source of my config, that I use in my Pipeline configuration. You'll notice that there's no source code files here, because now CircleCI config files don't need to live in the same place as the source code. Cool!

The source code files, that are checked out during the `checkout` command, live here: [checkout repo](https://github.com/jenny-miggin/checkout-repo)

## But wait, there's more!

Changes to this repo don't trigger a CircleCI pipeline. The trigger is based off of commits to another repo. 

The source code files, that are checked out during the `checkout` command, live here: [trigger repo](https://github.com/jenny-miggin/trigger-repo)

### TL;DR

This means that:

- CircleCI config lives in Repo A
- The code that is checked out during the checkout command lives in Repo B
- The repo that triggers a build lives in Repo C