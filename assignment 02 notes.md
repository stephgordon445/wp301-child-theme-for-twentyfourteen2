Assignment 02 Notes
=====================================

content-page.php
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