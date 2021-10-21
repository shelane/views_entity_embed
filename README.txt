CONTENTS OF THIS FILE
---------------------

 * Introduction
 * Requirements
 * Installation and Configuration
 * Maintainers

Views entity embed module allows you to embed views in textarea using WYSIWYG editor.

REQUIREMENTS
------------

- Editor and Filter or Link modules included with Drupal core.
- Embed module (https://www.drupal.org/project/embed)
- Entity Embed module (https://www.drupal.org/project/entity_embed)


INSTALLATION and CONFIGURATION
------------------------------

- Download module and store it in module folder or use composer ( composer require drupal/views_entity_embed) .
- Enable the module
- Enable the filter 'Display embedded views' for the desired text formats from the Text formats and editors configuration page. ( admin/config/content/formats )
If the Limit allowed HTML tags filter is enabled, add <drupal-views data-view-name data-view-display data-view-arguments data-embed-button> to the Allowed HTML tags.
- Go to Embed buttons administration page (admin/config/content/embed) and create a new button, which embedded type is 'Views'.
You can choose between the both options:

    * Filter which Views to be allowed as options:
    * Filter which Display to be allowed as options:

Only the selected views will be allowed to be embed by this Views embed button and for the Views Displays is the same. If you leave the options unchecked so all the views will be allowed.

- To enable the WYSIWYG plugin, move the views-entity-embed button into the Active toolbar for the desired text formats.
In WYSIWYG after click the Views Embed Button there are 4 steps

    * Select the view
    * Select the display
    * Checkbox for override the title
    * Populate the context filters ( if the view has)

MAINTAINERS
-----------

 * bibishani - https://www.drupal.org/u/bibishani
