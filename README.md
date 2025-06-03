# ICMS Recipe: Content Hub

> [!NOTE]
> @TODO: add Recipe description

### Useful commands
Copy the staged file to a temporary recipe config folder
```bash
mkdir -p drupal/packages/staged-config && \
git diff --name-only --cached | xargs -I{} cp {} drupal/packages/staged-config
```

Config Actions docos:
https://git.drupalcode.org/project/distributions_recipes/-/blob/1.0.x/docs/config_action_list.md


## TODO:
- [x] Handle translations
- [] validation errors: XYZ is not a supported key.
