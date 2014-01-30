Assignment 02 Notes
=====================================

content-page.php 01.30.14
--------------------

### Errors

I looks as though you didn't test your changes by loading the page. Please be sure to load the page to make sure it works. If you have the "WP_DEBUG" activated as mention in the previous notes below you will see the error and the line it is on.

You removed the wrong ";". You were referring to the line number I mentioned, though that line number changed when you removed a line above it. The issue mentioned below was on line 23 but is not on line 22. However, you still removed a ";" on line 23 which did not need to be removed and have created another error.

Try and see if you can use the WP_DEBUG setting mentioned below to diagnose the issue and make the fix. Going into your theme and blindly making changes with out testing will always lead to more errors and they will start to compound on top of each other and create more confusion. Always test your changes!

### Custom Fields

The assignment only mentions using the custom fields function "the_field()". The goal of adding the custom fields plugin was to give you a feel for utilizing a plugin for added functionality. I'm sure the plugin allows for much more, but it is best to work with the basics before moving into the more advanced features.

If you're able to utilize the plugin as mention in the assignment that would be enough.

Create a custom field named 'custom-title' and use it with the function the_field()

content-page.php 01.29.14
--------------------

### Errors
This file is throwing an error. You may need to activate error display in your wp-installation from the wp-confi.php file line 81. Activating errors was covered in the MAMP video. 

**Example of activate errors**

WordPress offers the ability to activate php errors from the wp-config.php. There are other ways to activate php error display, this is how wp makes it easy to activate it globally.

```
define('WP_DEBUG', true);
```

Once you have errors displaying you'll be able to target the errors.

[Codex Reference: http://codex.wordpress.org/Debugging_in_WordPress](http://codex.wordpress.org/Debugging_in_WordPress)

**Errors VS Warnings**

Activating php errors via WP_DEBUG will do more than just show 'errors'. It will also display warnings and usage of deprecated code, which is old wordpress functions that should no longer be used.

### line 20

This line contains "echo get_post_meta" which is incomplete. You need to either remove or complete the line of code. "get_post_meta" refers to a function that requires parameters. For more info check out the codex: [http://codex.wordpress.org/Function_Reference/get_post_meta](http://codex.wordpress.org/Function_Reference/get_post_meta)

### line 23

This line is the end of an if(){} statement. You have a ";" semicolon ending the statement which is not necessary.

### Wrap up

Once you have the error display activated you will always be able to see what is causing your issue. 

/fields directory
--------------------

You have a "fields" directory in your theme. I assume it may refer to the custom fields plugin that suggested during the assignment. Did you have any questions concerning the the "fields" directory?