# dokku custom scripts
dokku plugin to run custom scripts before and after build and deploy stages.

## requirements
- dokku 0.4.0+

## installation
```shell
dokku plugin:install https://github.com/martingregoire/dokku-custom-scripts.git custom-scripts
```

## usage
Add a folder `scripts` to the root of your app and place scripts into this folder. Name the scripts after the following trigger names:
- `scripts/dokku-pre-build`
- `scripts/dokku-post-build`
- `scripts/dokku-pre-deploy`
- `scripts/dokku-post-deploy`

See [Plugin triggers](http://progrium.viewdocs.io/dokku/development/plugin-triggers/) for a description of the triggers.
