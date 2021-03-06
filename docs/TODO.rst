=====
To do
=====

* 20091111: Replace leading tabs on literal blocks, just like for code blocks?

* 20091029: Matthew McCormick reports that the enumerated list is failing. Of course this is due to docutils 0.6, which creates its own complicated and byzantine environment to handle enumerated lists, without using ``enumerate``. For the moment, so as to handle backwards compatibility with docutils 0.5, we'll keep using our own environment.

* 20091028: RK reports that an image in a column aligns bad - it seems to get pushed to the bottom of the column. With docutils 0.6, and calling the latex image functions, it seems to be okay. But this loses our nice global resizing and centering of images. Maybe we can hack the right info onto the nodes.

* 20091027: A single script to regenerate all the examples?

* 20091024: MP advises that - at least with rst2beamer 0.6.4 and docutils 0.60 - subsections are missing Adobe bookmark. What does the docutils LaTeX writer do for this?

* 20091022: RK points out need for better testing. Difficult to test for fragments, but a demo document (test_all.rst) will do for the moment. What other features need to be in there?

* 20090810: The bullet overlay syntax can be made a lot simpler using a single optparse flag (e.g. ``--overlaybullets``). Also, the default behaviour should arguably be to *not* overlay bullets, but this will change the current default behaviour.

* 20090810: Desperately need maths markup. Sphinx has a pngmath extension module which may be suitable.
