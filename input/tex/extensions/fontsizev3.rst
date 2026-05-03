.. _tex-fontsizev3:

##########
fontsizev3
##########

The `fontsizev3` extension (nwe in v4.1.2) re-defines the various
font-sizing commands (like ``\tiny``, ``\small``, ``\large``, etc.) to
be the sizes that they were in MathJax v3 and in v4 prior to v4.1.2,
when they were corrected to be consistent with the sizes used in
actual LaTeX.  This extension is intended for those sites that have
legacy content where the old sizing values are critical to the layout.

This extension is **not** loaded automatically when the `autoload`
extension is used.  To load the `fontsizev3` extension explicitly, add
``'[tex]/fontsizev3'`` to the :data:`load` array of the :data:`loader`
block of your MathJax configuration, and add ``'fontsizev3'`` to the
:data:`packages` array of the :data:`tex` block.

.. code-block:: javascript

   window.MathJax = {
     loader: {load: ['[tex]/fontsizesv3']},
     tex: {packages: {'[+]': ['fontsizesv3']}}
   };

or, use ``\require{fontsizesv3}`` in a TeX expression to load it
dynamically from within the math on the page, if the
:ref:`tex-require` extension is loaded.

-----

.. _tex-fontsizesv3-commands:

fontsizesv3 Commands
--------------------

The `fontsizesv3` extension implements the following macros:
``\Tiny``, ``\tiny``, ``\scriptsize``, ``\small``, ``\normalsize``,
``\large``, ``\Large``, ``\LARGE``, ``\huge``, ``\Huge``


|-----|
