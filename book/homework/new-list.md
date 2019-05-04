# Add elements to the DOM

Let's practice what we learned by adding new content to the web page. We want to finish the web page by adding names of awesome women.

{% hint style='tip' %}
##### Hey Slacker!

Remember, we're here to help.
Join the KCWiT #codingandcocktails Slack Channel: [kcwit.slack.com](http://kcwit.slack.com)
{% endhint %}


1. Using Atom, declare a new array to hold the names of awesome women after the `brainSkills` array in _scripts.js_. You can use whatever variable name you want. 
   {% hint style='working' %}
<details>
<summary>
Need a little help? Expand this section for guidance. 
</summary> 
Type <code>const ladyDevs = [];</code>.
</details>
   {% endhint %}

1. Populate the array with names of women you met at Coding & Cocktails. If you can't remember any names, here's some awesome lady devs to use:
   * Grace Hopper
   * Evelyn Boyd Granville
   * Ada Lovelace
   * Barbara Liskov
   * Margaret Hamilton
   * Sister Mary Kenneth Keller

1. Find the declaration for the function `addDevSkill` at the top of _scripts.js_. After the `addDevSkill` function closing curly brace, declare a new function to use for writing the names of the lady devs to the DOM. Remember, function names are verbs and parameters are nouns.
      {% hint style='working' %}
<details>
<summary>
Need a little help? Expand this section for guidance. 
</summary> 
Create a new function and name it after the action (the verb). In this example, the action is `addLadyDev`. You can use <b>Function expression</b> or <b>Function declaration</b>. Your function should look something like this:

<pre>
<code class="lang-javascript">
const addLadyDev = function (ladyDev) {
};
</code>
</pre>
</details>
   {% endhint %}

   <!-- {% hint style='danger' %}
   If you didn't use the help section, you'll want to rename the function you created in this step to `addLadyDev` and the parameter to `ladyDev` before continuing.
   {% endhint %} -->

1. Between the opening and closing curly braces of your new function, type the following code to create a new list element, set the text, and add it to the DOM:
  
   ```js
   let listItem = document.createElement('li');
   listItem.innerHTML = <your function's parameter for lady devs>;
   document.getElementById("fellow-ladydevs").appendChild(listItem);
   ```
   {% hint style='info' %}
This is a sneak peek at a concept we'll cover in more detail next session-- DOM manipulation. Here we are creating a list dynamically in JavaScript and adding it to the webpage. Now you're extra prepared for next session!
   {% endhint %}

1. In the `document.addEventListener("DOMContentLoaded", ...)` function at the bottom of _scripts.js_, iterate through the new array and call your newly created function.   
   {% hint style='working' %}
<details>
<summary>
Need a little help? Expand this section for guidance. 
</summary> 
Take a look at how you iterated over <code>brainSkills</code> and called the <code>addDevSkill</code> function. You'll do the same for <code>ladyDevs</code> array and calling <code>addLadyDev</code> function.
</details>
   {% endhint %}

1. Save your file and start atom-live-server. Do you see the names of fellow LadyDevs? Upload a picture of your web page to Slack and show off your work!

<!-- trick markdown to give me a little space between these two sections of text -->
## 

## Checkpoint <span class="navigate-top"><a href="#top" title="Take me to the top of page"><i class="fa fa-chevron-circle-up" aria-hidden="true"></i></a></span>
Compare your _scripts.js_ against the answer key for your work. It might look a little different depending on spacing and names of Lady Devs.  
{% include "./checkpoint.html" %}