# APPtivity

The [finished app](http://codepen.io/baddeo/pen/ofqGk)

## Let's code

1. Find **CodePen**
* Sign up
* Create new pen
* Remember to **save** your pen(s) `⌘ + S`

## Structure

1. Set up the HTML box (hide the JS and CSS boxes)
* Explain `body` and `head` 
* Write all the content of our app 
* `h1` (useful for Google Fonts later)
* `p`
* `input`
* Difference between `value` and `placeholder`
* `button` with the same content of the `h1` to explain the concept of **markup**
* `p#message`
* Add `id` attributes to `input` elements

##### OPTIONAL 

* `a` links to share on TW and FB (rather important to learn how to make hyperlinks, and how to use `class` with eg: `a.link`)


## Style intro

Useful to show **selectors** and hide the `p`

1. `h1` centred
* `p`

        p#message
		{
		    display: none;
		}
* `button`: `color` and `background`
* [Google Fonts](https://www.google.com/fonts)  

##### OPTIONAL 

* [Normalize.css](http://necolas.github.io/normalize.css/)




## Break!



## Code a human

AKA *Robot time*

The idea is to engage people with an [easy task](http://pss.sagepub.com/content/early/2012/08/31/0956797612446024.abstract) before we challenge them with a demanding one

1. Let's pretend I'm a **robot** and you have to **code me**.
	* **Mission**: find an object in the room, pick it up.
	* I only understand these **commands**: `walk(steps)` and `turn(degrees)`
	* I can asnwer **questions**, only with a `yes` or `no`
* People usually start by giving you very *specific instructions* (eg: walk 3 steps, turn 45 degrees, walk 2 steps..)
* We can then make them their code more *abstract* and *flexible* with **logic** and **functions**.

If people are still puzzled, let them play [LightBot](http://lightbot.com/) for a bit.



## Behaviour

This is where things start to get really powerful!

1. Introduce `console.log`
* Include **jQuery** (explain *libraries*)
* Make `p#message` appear `jQuery("p").fadeIn()`
* Write a function which triggers when you click on the submit button
	
	    $("button").on("clik", doSomething)
	    
* We've got a **bug**. Let's fix it, by defining `function doSomething()`
* Make sure the function works, using `console.log` again
	
* Break down the app **behaviour**, introducing **comments**.
	
	    function doSomething()
	    {
	    	// 1. capture inputs
	    	
	    	// 2. make a choice
	    	
	    	// 3. display the choice
	    }

* Let's *google* `jquery get input value by id`.

	This will bring up the [jQuery.val()](http://api.jquery.com/val/) method, as well as the [quick answer from SO](http://stackoverflow.com/questions/4088467/get-the-value-in-an-input-text-box))

* Show people how to store the value of the first option in a **variable** `var option1 = ...` (because computers are **forgetful**, they won't **remember** unless you tell them to) 
* Ask people to store the value of `option2` in another variable.

* Let's see if we can display a **message**. 

	We'll use `option2` for now. 
	
	Introduce **string concatenation**.
	
	`$("p#message").html("You should " + option2)`
	
	
* Talk about [**Clarke's third law**](http://en.wikipedia.org/wiki/Clarke's_three_laws) `Any sufficiently advanced technology is indistinguishable from magic` to introduce the next step. We could develop an algorithm vased on various	APIs, however for now we'll just ask the computer to **make a random choice** and make it look like it's clever.

* Let's *google* `JS function to get random number`.
	
	One of the first results will be from [StackOverflow](http://stackoverflow.com/questions/1527803/)

* Introduce **branching logic**.	
* Display the **choice** (swap `option2` with `choice`)
* Bonus: make the message *motivational* with `f*****` or similar 


#### OPTIONAL

1. Make `p#message` fade out on click

## Dress code

1. CSS **final touches**

	* `font-size`
	* `font-weight`
	* `width`
	* `margin`
	* `padding`
	* tranparency
	* `border-radius`
	* `background-image`
* Click on **Share** and then send to your phone
* Make the app look proper on a phone. Google `how to stop phone zooming out pages`
* Make the app **full screen**. Google `how to hide address bar in mobile browser` and you should find [this tutorial](http://www.html5rocks.com/en/mobile/fullscreen/) 
* Add the app to your phone's **home screen**
 
         <link rel="apple-touch-icon" href="http://i.imgur.com/ln9kdl3.png">
  
#### OPTIONAL         	

* `-webkit-appearance: none;` to get rid of inner shadows in `input`



## What next?
 
Hook it to an **API** (eg: weather, maps, videos, music, [unistats](http://unistats.direct.gov.uk/)...)


### Debug


