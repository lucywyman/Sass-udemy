Compiling your first Sass file
==============================

Welcome to the course!  In this exercise we'll walk through compiling
your first Sass script into CSS. :code:`1.scss` is our main sass file which we 
will be compiling into CSS. 

To compile :code:`1.scss` once, run

.. code-block:: none

	$ sass 1.scss 1.css
	$ ls
	1.css  1.css.map  1.scss  _partial.scss

And you're done! If you run :code:`ls` you should see output just 
like the one above. You now have a file, :code:`1.css`, which you 
can include in your project!  There should also be a :code:`1.css.map`
-- this is a sourcemap, which you can use for debugging Sass in your
browser. Don't worry about it too much for now, we'll talk more about 
it later in the course!

You can also make the output file named whatever you would like, for
instance we could also run

.. code-block:: none

	$ sass 1.scss output.css

This is generally a bad idea, as it's difficult to tell which Sass
script this CSS file came from, but it is possible if you need to use 
it!

You can also watch a Sass script for changes, which is especially
useful for development. There are several project-specific tools (like
grunt) which will also do this for you, but Sass itself has the 
capability to automatically recompile your script every time you make 
a change.

.. code-block:: none

	$ sass --watch 1.scss:1.css 
	>>> Sass is watching for changes. Press Ctrl-C to stop.
      	write 1.css
	  	write 1.css.map


Congratulations on compiling your first Sass script!  In the following
weeks we will go over what each element in :code:`1.scss` is, so 
stay tuned!
