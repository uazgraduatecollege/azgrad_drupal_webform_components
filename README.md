# AZ Grad College Webform Components
## For Quickstart 2 / Drupal 9+

Provides webform components, especially select options, from dynamic JSON sources.

- AZ Graduate Programs
- AZ Degree-Seeking Graduate Programs
- AZ Doctoral Programs
- AZ Doctoral Minors
- AZ Masters Programs
- AZ Accelerated Masters Programs
- AZ Certificate Programs
- AZ Terms
- AZ Current and Future Terms
- AZ Campuses
- AZ Locations

## Installation

Assuming you have a Quickstart 2 site's git repository cloned, edit your site's 
`composer.json` file.

Add the following to the `repositories` section:

```json
  {
    "type": "vcs",
    "url": "git@github.com:uazgraduatecollege/azgrad_drupal_webform_components.git"
  }
  ```
And add the following to the `require` section:

```json 
  {
    "uazgraduatecollege/azgrad_drupal_webform_components": "dev-main"
  }
```

Commit your changes and re-initialize you site.

If using a site cloned from Pantheon, delete your `composer.lock` file before
committing your changes and then `git push` back up to the pantheon remote.

## Configuration 

Enable the by navigating to your site's `Admininistration => Extend` and clicking 
the AZ Grad Webform Components module.

Alternatively, enable using terminus:

```sh
$ terminus remote:drush en azgrad_drupal_webform_components 
```

The components provided by this module should now be ready to use in Drupal webforms.

## Notes

