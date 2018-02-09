Document Object Model and JavaScript
------------------------------------

Chapter Contents
~~~~~~~~~~~~~~~~

.. toctree:: 
    :maxdepth: 1

    javascript

Introduction
~~~~~~~~~~~~

JavaScript is a general-purpose programming language that can be used to write many kinds of computer programs. However, it has also become the defactor scripting language of the World Wide Web. In fact, its destiny is so tightly intertwined with the Web, that it can be used to manipulate every element, attribute, and character of text in an entire Web document.

It utilizes what's called the **Document Object Model**, or **DOM**. The DOM is a way of thinking about and structuring an HTML document in such a way that we can locate different parts of it by digging down through it from the very top. Imagine a web page as structured like this:

.. image:: images/flow.png
   :width: 100%


We can use JS to react to events, add and delete elements, change styles, and even content. The interface between HTML and JS gives total control of all aspects of the web page. This is both good and bad, by the way.

The purpose of this chapter is to give a *brief* introduction to JavaScript the language, but with a particular emphasis on the way it interacts with the DOM.

First, a quick example:

.. code-block:: html
    :linenos:

    <body>

    <h1 id="site-heading">
        Hello World!
    </h1>

    <script>
        document.getElementById("site-heading").innerHTML = "Hello JS!";
    </script>
  
    </body>

To see this in action, check this jsfiddle:

.. raw:: html

    <script async src="http://jsfiddle.net/erickuha/ura0xxk1/embed/result/"></script>

The purpose of these tutorials is not to make you an expert at general-purpose programming. We'll learn just enough JavaScript syntax to know how to use it to manipulate the DOM for building web pages. That said, some basic concepts like variables and sequential execution are covered on the next page.
