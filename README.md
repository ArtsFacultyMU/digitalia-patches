# digitalia-patches
This module holds all patches used on any of the Digitalia platforms. To apply a patch, include it in the composer.json of the platform and the module composer-patches must be installed.

Clone this module to /var/www/html/drupal
```
git clone-<your_name> git@github.com:ArtsFacultyMU/digitalia-patches.git patches
```

If a specific patch needs to be modified after an update, create a new patch and add the version of the module or drupal/core to the patch name.

| Patch        | Module       | Reason       |
| ------------ | ------------ | ------------ |
| form.inc.patch | drupal/core | Datafield error fix: display references in select list |
| SqlContent.patch | drupal/core | Datafield error fix: save references in select list |
| ComplexDataNormalizer.patch | drupal/core | Datafield/Workbench fix: normalize non-object fields properly |
| Xss.patch | drupal/core | Allow `fieldset` and `legend` tags |
| persistent_identifiers.patch | drupal/persistent_identifiers-persistent_identifiers | Create handle automatically on node save/creation |
| MetaNameBase.patch | drupal/metatag | Make all field multiple |
| gnode.links.action.patch | drupal/group | Allow adding entities to group from non-default views |
| group_term.links.action.patch | drupal/group_term | Allow adding entities to group from non-default views |
| EntityComparisonAddGroupCode.patch | drupal/entity_comparison | Add Group Code |
| hdl.module.patch | drupal/persistent_identifiers-persistent_identifiers | Reenable qualifier field in configuration |
| HideWhenNoFilters.patch | drupal/facets | Add processor HideWhenNoFilters to hide empty facet summary |
| FacetsFilter.patch | drupal/facets | Show empty facets |
