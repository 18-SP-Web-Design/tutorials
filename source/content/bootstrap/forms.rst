Form
----

Another obvious thing that we will want to do is build forms. If we practice with this a bit, then we will have enough knowledge to use any of the other widgets and style options that come packaged up with Bootstrap.

First, let's look at building a basic password entry form (this will be largely non-functional, of course, since we're not building a backend, but the basic principle is the same).

Here are the classes we'll look at:

#. :code:`.form-group` should wrap a form element and its label to logically form it as one item.
#. :code:`.form-control` is kind of a catch-all class for textual elements like :code:`<input>`, and :code:`textarea`.
#. :code:`.btn btn-default` because you gotta have buttons. As a sidenote, you can use these classes on ordinary anchor tags to make them look like buttons.
#. :code:`.form-check-input` for checkboxes.

In addition to these, there will be a few label classes that are also included in Bootstrap, so look for those as well.

Start with a basic Bootstrap template and add the following code:

    .. code-block:: html
        :linenos:

        <div class="container">
            <form>
            <div class="form-group">
                <label for=="emailBox">Email Address</label>
                <input type="email" class="form-control" id="emailBox" placeholder="Enter email" aria-describedby="emailHelp" />
                <small id="emailHelp" class="form-text text-muted">Your privacy is important to us.</small>
            </div>
            <div class="form-group">
                <label for="passwordBox">Password</label>
                <input type="password" class="form-control" id="passwordBox" placeholder="Password" />
            </div>
            <div class="form-check">
                <input type="checkbox" class="form-check-input" id="checkbox" />
                <label class="form-check-label" for="checkbox">Remember me</label>
            </div>
            <button type="submit" class="btn btn-primary">Submit</button>
            </form> 
        </div>


Examine the code carefully. In most respects, this is like any other form code. But we've divided it up into small div wrappers to apply Boostrap styles. There are a number of differences, but if you are getting familiar with the way HTML and CSS play with each other, adding in these simple classes has a pretty dramatic effect on the look and feel of a form.

For example, the above code without Bootstrap:

    .. image:: images/form_no.png
        :width: 100%

And with the Bootstrap CDN added:

    .. image:: images/form.png
        :width: 100%
