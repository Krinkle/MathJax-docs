.. _dark-mode:

#################
Dark Mode Support
#################

As of v4.1.0, MathJax provides support for browsers using dark-mode
system settings.  MathJax dialogs, menus, and expression explorer all
will use a dark-mode color set automatically when dark-mode is enabled
in the system preferences.

This works well when the webpage itself has dark-mode support.  But if
not, then the explorer dark-mode colors can make the text somewhat
harder to read.  For those pages, MathJax v4.1.1 and later provides an
extension to disable dark mode.

To disable the dark-mode colors, include ``ui/no-dark-mode`` in the
:data:`load` array of the :data:`loader` section of your MathJax
configuration object:

.. code-block:: javascript

   MathJax = {
     loader: {load: ['ui/no-dark-mode']}
   };


This will prevent dark mode from being used in dialogs and the
explorer; menus will remain in dark mode, however, but that should not
cause an issue, as the menu's dark color scheme also works well in
light mode.

|-----|
