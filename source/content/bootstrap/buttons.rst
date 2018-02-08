Buttons and Icons
-----------------

To include everything there is to talk about in Bootstrap eventually begins to look like just listing all of the classes and showing examples of how they work. Once you have the basics down, there's really little point in doing that since you can just browse the `documentation <https://getbootstrap.com/docs/4.0/getting-started/introduction/>`_ to find the component you're looking for.

But there is one other thing that warrants at least a brief tutorial: Icons. Bootstrap used to include an icon font by default, but in Bootstrap 4, it was removed. Instead, they recommend any number of icon fonts that are available (often for free) elsewhere and which have easy Bootstrap integration.

First of all, what do we mean by "icon"? Well, in modern design, an icon is a specialized graphical element which can convey meaning without being a word. We have been using icons for a long time. We all know that to save a document, you usually click on the icon that looks like an old-style computer disk. And there are some equally universal icons out there creating a sort of glyph meta-language.

A number of companies have made icons into a design language. For the sake of this tutorial, we will use the icon font designed by `Font Awesome <https://fontawesome.com/>`_, since they are kind enough to use a CDN to distrubte it.

We're going to see how to add icons to buttons and to use them as buttons in themselves. We'll combine their functionality with Bootstrap for very nice results. So let's get started. 

#. Open your basic Bootstrap template and add the Font Awesome CDN to the :code:`<head>` element:

   .. code-block:: html

       <script defer src="https://use.fontawesome.com/releases/v5.0.6/js/all.js"></script>

#. Let's start with a simple button. Let's say you want to create a download link. You can do this in Bootstrap very easily:

   .. code-block:: html
       :linenos:

       <div class="container">
           <h2>Download the file here:</h2>
           <a class="btn btn-primary" href="#">Download</a>
       </div>

#. This will create a pretty standard button:

   .. image:: images/icon1.png
       :width: 50 %
       :alt: Button With no Icon 

#. Next, we want to create an icon which will add visual appeal and instant recognition to the button. First, we need to find a suitable icon to use. You've added the Font Awesome library of gliphy icons to the page, but there are over 900 free icons in the library. So, let's go digging. Head over to their website and search through the `free icons <https://fontawesome.com/icons?d=gallery&q=Down&m=free>`_. For example, type the word "Download" into the search bar and see what comes up:

   .. image:: images/icon2.png
       :width: 100 %
       :alt: Searching for an icon

#. All you really need is to see the name of the icon which is right underneath it. However, if you click on the icon, it will show you some examples of the icon in action. Font Awesome's recommended way of including an icon looks like this:

   .. code-block:: html
       :linenos:

        <i class="fas fa-download"></i>

   Simply add this bit of code right into your link:

   .. code-block:: html
       :linenos:

       <a class="btn btn-primary" href="#"><i class="fas fa-download"></i>Download</a>

   And observe the results:

   .. image:: images/icon3.png
       :width: 100 %
       :alt: With Icon

Note: 
~~~~~~

Font Awesome's convention of using :code:`<i>` tags to denote an icon is nice because it is brief succinct, however it is not semantically correct since that tag already has a semantic meaning in HTML. Technically, it would be more correct to use a :code:`<span>` tag, however, you will almost certainly not notice any ill effects from using the i tag since the way Font Awesome's JavaScript library works, it simply replaces the entire element with an :code:`<svg>` element anyway. So use the i. It's nice and simple.

Make it fancy
~~~~~~~~~~~~~

Font Awesome's `documentation <https://fontawesome.com/how-to-use/svg-with-js#basic-use>`_ is short but has plenty of interesting options for you to try.

And for the most part, they are accomplished simply by *adding classes* to the element with the icon. It's as simple as that.

Among the features outlined in their documentation are:

* Icons inherit CSS styling:

  .. code-block:: html

      <div style="font-size:3em; color:GoldenRod">
          <i class="fas fa-hand-spock"></i>
        
      </div>


  .. image:: images/icon_spock.png

* Icons can be animated:

  .. code-block:: html

      <div class="fa-3x">
          <i class="fas fa-sync fa-spin"></i>
      </div>

  .. raw:: html

      <svg class="svg-inline--fa fa-sync fa-w-16 fa-spin" aria-hidden="true" data-prefix="fas" data-icon="sync" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" data-fa-i2svg=""><path fill="currentColor" d="M440.935 12.574l3.966 82.766C399.416 41.904 331.674 8 256 8 134.813 8 33.933 94.924 12.296 209.824 10.908 217.193 16.604 224 24.103 224h49.084c5.57 0 10.377-3.842 11.676-9.259C103.407 137.408 172.931 80 256 80c60.893 0 114.512 30.856 146.104 77.801l-101.53-4.865c-6.845-.328-12.574 5.133-12.574 11.986v47.411c0 6.627 5.373 12 12 12h200.333c6.627 0 12-5.373 12-12V12c0-6.627-5.373-12-12-12h-47.411c-6.853 0-12.315 5.729-11.987 12.574zM256 432c-60.895 0-114.517-30.858-146.109-77.805l101.868 4.871c6.845.327 12.573-5.134 12.573-11.986v-47.412c0-6.627-5.373-12-12-12H12c-6.627 0-12 5.373-12 12V500c0 6.627 5.373 12 12 12h47.385c6.863 0 12.328-5.745 11.985-12.599l-4.129-82.575C112.725 470.166 180.405 504 256 504c121.187 0 222.067-86.924 243.704-201.824 1.388-7.369-4.308-14.176-11.807-14.176h-49.084c-5.57 0-10.377 3.842-11.676 9.259C408.593 374.592 339.069 432 256 432z"></path></svg>

They can also be resized, rotated, translated, and nested on top of each other. Experiment and see what you can create with icons. They're basically the future of language at this point.
