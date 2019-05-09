# **TASKS**

## Preliminary 

1. Learning basic Linux
    1. Reach at least lvl 10 in this game: [Overthewire](http://overthewire.org/wargames/bandit/) (~ 2-2,5 hours)

2. Learning Markdown
    1. Finish this tutorial: [Markdown](https://www.markdowntutorial.com/) (~ 1 hour)

3. Learning GitHub and Git
    1. Finish this tutorial: [GitHub](https://guides.github.com/activities/hello-world/) (~ 30 mins)
        1. Some help: https://rogerdudler.github.io/git-guide/
        2. Some more help: http://marklodato.github.io/visual-git-guide/index-en.html

4. Learning node.js: Choose one of the following
    1. (Free) Simple tutorial: [Tutorialspoint](https://www.tutorialspoint.com/nodejs/index.htm)
    2. (Free) More about the language and frequently used patterns: [Eloquent](https://eloquentjavascript.net/)
    3. (Paid) [Udemy](https://www.udemy.com/the-complete-nodejs-developer-course-2/) (> 10 hours)
No matter what tutorial, you choose make sure to learn what is:
* The language syntax
* Working with local packages, npm, publishing packages
* Asynchronous programming with callbacks, promises
* JSON format
* Handling basic HTTP requests

5. Learning JSON Schema:
    1. Finish this tutorial: [JSON-schema](https://json-schema.org/understanding-json-schema/) (~ 4 hours)
    	1. During this tutorial, keep writing small JSON Schemas and validating them with an online JSON Schema validator. [An example](https://www.jsonschemavalidator.net/)

### WoT Tutorial

1. Understand this standard: [Thing Description](https://www.w3.org/TR/wot-thing-description/)
	1. This standard is part of Web of Things, which is detailed in [the architecture document](https://w3c.github.io/wot-architecture/). This document can help you to understand the concept rather than the document format. 
	2. Web of Things is a concept that is being standardized by W3C. However, there are other people/organisations talking about it. Do not copy them but use them only to learn the concept. Some examples are from Mozilla and the book called Building the Web of Things.

2. Write a TD of a coffee machine that meets these requirements:

* name and id up to you to decide
* I should be able to read the state of the machine, like brewing, grinding, error etc.
* I should be able to brew a coffee of my choice by sending some request. You can be creative
about what your machine offers
* I should be able stop a coffee brewing process by sending some request. Just for fun, this should be done with a CoAP request.
* I should be able to turn it off remotely, only to turn it on manually later on
* It should notify me when there is not enough water, coffee beans, when its bin needs to be
emptied or in case of an error X
* I should be able to see how much water, coffee beans are left, how full the bin is

This is intentionally vague, I am expecting you to come up with something. It doesn't have one correct answer. 

Test your TD with [Playground](http://plugfest.thingweb.io/playground/). If you think that your TD is actually valid but Playground says otherwise, write a GitHub issue.

* In the end, commit this TD to the GitHub of Playground under WebContent/Examples/Valid. How you should do this is up to you to figure out but should not be a problem if you did the GitHub tutorial ^^
  
3. Install [node-wot](https://github.com/eclipse/thingweb.node-wot) and whatever development environment you want. Create the coffee machine server code. Of course, you won't interact with the hardware but it should respond to requests like its TD says and node-wot should produce a TD that is similar to the TD you wrote before. 
	1. To interact with it, you can use Postman.
	2. Then test your implementation with [WoT Test Bench](https://github.com/tum-ei-esi/testbench). **Warning** This tool might be a bit buggy. Ask Ege immediately if you see unintended behavior.

4. Now that you have a Thing working, think of a mashup idea involving this Thing and another one you can think of. Possibilities are endless so keep it simple. This is intentionally left vague. You would need to understand what a mashup is then decide where the mashup code will work and how many entities should be involved.

 Before proceeding, check out the following tools: [WoT webui](http://plugfest.thingweb.io/webui), [virtual-thing](https://www.npmjs.com/package/virtual-thing)