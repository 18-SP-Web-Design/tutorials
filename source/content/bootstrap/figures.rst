Figures
-------

What would a web page be without multimedia? Especially the most fundamental of media: images.

Bootstrap comes with several classes and other options for handling images within containers, columns, and other Bootstrap elements.

Build into HTML5 is the :code:`<figure>` element, which is nicely semantic and highly useable and allows for nesting of other useful elements like captions.

Bootstrap simply works to build on these built-in elements.

The basic classes are:

#. :code:`.figure` used to apply Bootstrap theming to the :code:`<figure>` tag.

#. :code:`.figure-img` Along with the a few other classes, like :code:`.img-fluid` and :code:`.rounded` to nicely format images and make the responsive.

#. :code:`.figure-caption` added to a :code:`<figcaption>` element.

For example. Inside a basic Bootstrap template, you have the following code:

    .. code-block:: html
        :linenos:

        <div class="container">
            <figure class="figure">
                <img src="discovery2.jpg" class="figure-img img-fluid rounded" alt="Discovery!"/>
                <figcaption class="figure-caption">The USS Discovery</figcaption>
            </figure>
        </div>

This code results in a nicely formatted image and caption which will automatically scale to fit whatever browser it's rendered in. It will also easily scale to fit inside of a Bootstrap column or any sized container you like.

    .. image:: images/figure.png
        :width: 100%

Once again, the `documents <https://getbootstrap.com/docs/4.0/content/figures/>`_ have more information.
