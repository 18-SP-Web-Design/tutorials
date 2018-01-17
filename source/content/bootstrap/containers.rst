Containers
----------

So how do I use Bootstrap? If you've gotten this far, then we'll assume that you know about CSS and especially CSS classes. The majority of what you'll do when you use Bootstrap to enhance your Web page is simply apply classes to HTML tags that are already there.

You will, however, often have to surround chunks of code with *div* tags in order to do this. This does, to some extent, violate the semantic philosophy of HTML, but, the end result is so nice that the compromise is kind of worth it.

There are two main container classes in Bootstrap:

#. :code:`.container` is a fixed-width container that takes up the strip in the center of the page. It's the one you'll most often use.
#. :code:`.container-fluid` is a container that fills the entire width of the viewport (the browser window).

In addition to these, we will look at the basics of the Bootstrap grid system and the :code:`.jumbotron` class.

**Note:** You don't need containers to use a lot of Bootstrap's built-in widgets, however, you will need it to use the really handy Bootstrap grid system. Let's try it:

#. Clone the repository for this tutorial if you have not already //TODO link to repo
#. The majority of Bootstrap's styling is done by surrounding various code snippets with :code:`<div>` tags using Bootstrap classes. So let's surround the first part of the page with a :code:`<div` and add the :code:`.jumbotron` class as well as center the text::
   
    <div class="jumbotron text-center">
        <h1>Welcome to my page!</h1> 
        <p>Feel free to look around and stay a while.</p>
    </div>

#. Reload the web page and observe the results. There plenty of ways that we can use the jumbotron container. You can add a background image to it to add visual interest, for example.
#. Next, Surround the rest of the page content with another div tag and the :code:`.container` class, like so::

    <div class="container">
    ... Your Code Here ...
    </div>

#. Reloading the page will give you this:

   .. image:: images/container1.png
        :width: 100%


