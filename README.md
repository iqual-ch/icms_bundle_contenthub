# ICMS Recipe: Content Hub

> [!NOTE]
> @TODO: add Recipe description

### Useful commands
Copy the staged file to a temporary recipe config folder
```bash
git diff --name-only --cached | xargs -I{} cp {} drupal/recipes/staged-config
```

Config Actions docos:
https://git.drupalcode.org/project/distributions_recipes/-/blob/1.0.x/docs/config_action_list.md


## TODO:
- [] Handle translations
- [] validation errors: XYZ is not a supported key.
