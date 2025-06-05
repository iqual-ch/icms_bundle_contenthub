# ICMS Recipe: Content Hub

> [!NOTE]
>
> @TODO: add Recipe description

### Useful commands
- Install recipe:
  ```bash
  composer require iqual/icms_bundle_contenthub && drush recipe ../packages/icms_bundle_contenthub
  ```
- `[DEV]` Reset recipe during dev (remove staged config):
  ```bash
  drush cim -y && drush recipe ../recipes/icms_bundle_contenthub
  ```
- `[DEV]` Copy the staged file to a temporary recipe config folder
  ```bash
  mkdir -p drupal/packages/staged-config && \
  git diff --name-only --cached | xargs -I{} cp {} drupal/packages/staged-config
  ```

Config Actions infos:
- [Config Actions list](https://git.drupalcode.org/project/distributions_recipes/-/blob/1.0.x/docs/config_action_list.md)
- ["You don't want to update dependencies using recipes"](https://www.drupal.org/project/distributions_recipes/issues/3348991)
- [CA array operations (patch installed)](https://www.drupal.org/project/drupal/issues/3365328#comment-15864385)

## TODO:
- [x] Handle translations (patch installed)
- [ ] validation errors: XYZ is not a supported key (Flat Taxonomy schema issue?).
- [ ] Test overlapping config with other recipes (handle existing config)
- [ ] Removing drupal/conditional_fields and use State API instead (blokkli issue, CF not applied)
