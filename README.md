# How to create keyword ban platform

This a guide to create the a private post type with custom fields on the admin dashboard of WP.

## You will need to install _two_ plugins:

1. Custom Post Types UI created by WebDevStudios
2. Advanced Custom Fields created by Delicious Brains

### Setting up Custom Post Types

First, activate your plugins and create a private custom post type using the Custom Post Types UI (CPTUI). Start by naming your Post Type Slug, e.g., "keyword_ban", or whatever is most intuitive for your project.

Next, assign your plural and singular labels, e.g., "Keywords"/"Keyword".

Before clicking "Add Post Type", scroll down to settings near the bottom and adjust the "Public" setting to "false", and also check only "Title" and "Custom Fields" under the "Supports" option. Finally, click "Add Post Type" and you should see it pop up in your admin menu as a tab.

### Setting up advanced custom fields

After you have created your Custom Post Type, go to the advanced custom fields(ACF) plugin and click "Add New". You can title it however you'd like. As a suggestion: "Keyword Categorizer". Then, click "Add Field" and label it "Keyword". Set the "Field Type" to "Text"; you can choose to require it or not. Next, click "Add Field" again and label it what you would like; change the "Field Type" to "Radio Button". Again, choose to require it again or not, and then add the choices you would like to have for your keywords. Next, under "Location" set "Show this field group if" to "Post Type" "is equal to" "**\_**"(whatever you named you CPT).

### You are now ready to add your keywords

Once you go into your CPT and click "Add New", you should see the custom fields you just created. The title input will be helpful because you can name it your keyword and it'll show it in the list on your CPT page, otherwise you will get a list full of "Auto Draft" items because there is no link between your custom field and the title at this point.

As a note, your CPT should be private from when you created it, but also make sure you click private next to "Visibility" when adding a new keyword.
