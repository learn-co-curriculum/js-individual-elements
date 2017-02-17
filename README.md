## Working with Individual Elements

## Introduction

In the previous lesson, we learned that JavaScript allows us to interact with the Document Object Model, which allows us to change what displays in a browser.  In this section, we will look at some of the more common Javascript methods for interacting with the Document Object Model.

## Don't memorize. Instead, read documentation.

We are about to learn a number of methods.  Don't feel like you have to memorize these methods.  If you're coding, you're on a computer, which means that you have access to Google.  Right now, type into Google:

  `common JavaScript methods interact with dom`

Or, just click [here](https://www.google.com/webhp?sourceid=chrome-instant&ion=1&espv=2&ie=UTF-8#q=common+javascript+methods+interact+with+dom). 

You will see a number of resources in the search results.  For JavaScript, resources the Mozilla Developer Network (MDN) is an excellent resource.  If you click on the search result from [MDN](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction#Core_Interfaces_in_the_DOM), you will find an article with a table of contents.  You can click on [Core Interfaces in the DOM](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction#Core_Interfaces_in_the_DOM) and see a list of common methods.  

Because information about programming is so accessible, we should lean on Google as an extension of our memory.  However, what we need to do is read through documentation, and go through courses like this one, so that we can develop an intuition for what methods and capabilities Javascript will provide to us.  

In this lesson, we will go through some of Javascript's most common methods for interacting with the DOM.  

### Selecting Elements

There are three common ways to select elements in JavaScript.

* document.getElementById
* document.getElementByClassName
* document.querySelector

Let's practice selecting html using these methods.  Below, you can see some sample HTML.

<div>
  <div class="hello">
    <h2 id="foobar"> This is sample HTML </h1>
    <p class="my-sample-html"> More sample HTML </h1>
  </div>
</div>

Now our task is to select the phrase `This is sample HTML` above using the getElementById method.  Ok, so if we are going to select the content above by id, we first need to know what that HTML element's id is.  To do this, hover over the element, and click inspect.  You will know that the correct element is selected because when your mouse hovers over the element, the element you are interested in turns blue.  Ok, so inspecting the element, we see the id.  Then we need we need to use the method `document.getElementById` to select it.  

In programming (and in life), we oftentimes guess when we don't know the answer.  The beautiful thing about programming is that nothing bad happens if you guess incorrectly.  Let's try guessing how to use the `document.getElementById` method to select h2 element with the sample text, "This is sample HTML".  So open up the console (press command+shift+c) and give it a shot.  

> Note: "You miss 100% of the shots you don't take."  - Wayne Gretzky

It worked, yes?

Or it didn't.

Either way, let's discuss.

The way we select this element by it's id is simply with `document.getElementById('user-content-foobar')`.  So we provide the id, and place it in quotes.  Either single quotes or double quotes will work.  

Now let's try using the method `document.getElementByClassName` to select the element enclosing the text `More sample HTML`.  A lot of programming is seeing one solution, and then trying to generalize a pattern.  Again, oftentimes we are wrong in what we think that pattern is.  It's a skill we develop over time.

Here the to selecting an element seems to be:
  1. Inspect the element to determine how to identify the element
  2. Then place the relevant attribute value between the parentheses of the method name

Let's try it.  Once again, we right click on the element we are interested in.  We see that the class name attribute of that element is `my-sample-html`.  So we open up our developer console, and take another good old fashioned guess.

Eventually...

after enough attempts...

and some luck...

you try

`document.getElementByClassName('my-sample-html')`

### Query Selector

Now, selecting an element by a query selector is slightly more complicated than selecting an element using one of the previous two methods, but don't worry you'll learn to love it.  But first, a look back.

<iframe height='265' width="125" scrolling='no' title='js and the web' src='//codepen.io/flatiron/embed/ggyKpb/?height=265&theme-id=0&default-tab=html,result&embed-version=2&editable=true' frameborder='no' allowtransparency='true' allowfullscreen='true' style='width: 100%;'>See the Pen <a href='https://codepen.io/flatiron/pen/ggyKpb/'>js and the web</a> by Jeffrey Katz (<a href='http://codepen.io/flatiron'>@flatiron</a>) on <a href='http://codepen.io'>CodePen</a>.
</iframe>

