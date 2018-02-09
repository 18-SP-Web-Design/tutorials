Intro to JavaScript
-------------------

As mentioned earlier, JavaScript is a general-purpose programming language. It doesn't have to be used for web development, but it does have a few advantage that make it ideally suited to the task. First, it's cross-platform, meaning that it can be executed on any computer in the world (for the most part). Second, it is simple enough and lightweight enough that it can be deployed as a package in a web browser, and indeed, every web browser worth using has a JS parser built-in. Lastly, JavaScript was in the right place at the right time. It's easier to learn that Java, and it got its start just as a new, less complex language (than Java) was needed for web-scripting.

So how do I do stuff with JS?

Variables
~~~~~~~~~

Think of a variable as a container that you put things in. Almost all programming languages have some way of storing a value for later use and JavaScript uses variables. To declare a variable, you use the :code:`var` keyword:

.. code-block:: js

    var myName;

Note, that when you create a variable, it is initially empty. To store something in it, we use the **assignment operator**, :code:`=`. 

.. code-block:: js

    myName = "Eric";

You can combine these into one line like this:

.. code-block:: js

    var myName = "Eric";

Notice that JavaScript uses semicolons to terminate all lines of code. There is some wiggle room with this rule, but it's probably a good idea to get into the habit as early as possible.

Data Types
~~~~~~~~~~

There are several basic data types that JavaScript supports. For the purposes of these tutorials, we will only use a couple, but here's a rundown of the most common ones:

+----------+-----------------------------------------------------------------------------------------+---------------------------------------------+
| DataType | Description                                                                             | Syntax                                      |
+==========+=========================================================================================+=============================================+
| String   | Just plain text. Strings of characters                                                  | :code:`var myName = "Eric";`                |
+----------+-----------------------------------------------------------------------------------------+---------------------------------------------+
| Number   | Numbers obey most algebraic principles                                                  | :code:`var myNum = 6;`                      |
+----------+-----------------------------------------------------------------------------------------+---------------------------------------------+
| Boolean  | A true/false value.                                                                     | :code:`var myBool = true;`                  |
+----------+-----------------------------------------------------------------------------------------+---------------------------------------------+
| Array    | A way of storing multiple values in one variable                                        | var myArray = [1, 'Eric', true, 15]         |
+----------+-----------------------------------------------------------------------------------------+---------------------------------------------+
| Object   | Objects are everything else. This will be important when we start manipulating the DOM. | myDiv = document.getElementById("someDiv"); |
+----------+-----------------------------------------------------------------------------------------+---------------------------------------------+


