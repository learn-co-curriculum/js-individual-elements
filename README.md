## Working with Individual Elements

## Introduction

In the previous lesson, we learned that JavaScript allows us to interact with the Document Object Model, which allows us to change what displays in a browser.  In this section, we will look at some of the more common Javascript methods for interacting with the Document Object Model.

## Don't memorize. Instead, read documentation.

We are about to learn a number of methods.  Don't feel like you have to memorize these methods.  If you're coding, you're on a computer, which means that you have access to Google.  Right now, type into Google:
  `common JavaScript methods interact with dom`

You will see a number of resources in the search results.  For JavaScript, resources the Mozilla Developer Network (MDN) is an excellent resource.  If you click on the search result from (MDN)[https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction#Core_Interfaces_in_the_DOM], you will find an article with a table of contents.  You can click on [https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction#Core_Interfaces_in_the_DOM](Core Interfaces in the DOM) and see a list of common methods.  

Because information about programming is so accessible, we should lean on Google as an extension of our memory.  However, what we need to do is read through documentation, and go through courses like this one, so that we can develop an intuition for what methods and capabilities Javascript will provide to us.  

In this lesson, we will go through some of Javascript's most common methods for interacting with the DOM.  

### Selecting Elements

There are four common ways to select elements in JavaScript.
  * document.getElementById
  * document.getElementByTagName
  * document.getElementByClassName

<div >
  <div class="hello">
    <h1 id="foobar"> Hello </h1>
    <p> Here is a paragraph </h1>
  </div>
</div>
