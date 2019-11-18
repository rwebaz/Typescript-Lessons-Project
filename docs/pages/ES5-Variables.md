---
title: ES5 Variables
layout: default
excerpt: The need to contain the scope of the variable(s) declared in `ES6` is a top priority ...
description: Place the intro paragraph ie.) the 'synopsis' here ...
repo: Typescript-Lessons-Project 
ver_date: 11-17-19
navigation_weight: 8
categories: page
---
{% include toc.md %}

## ES5 Var

In the past ES5 specification, even if a variable was assigned inside of a code block, for example:

```liquid
{% raw %}
function hoist(x){
  var inside = x + 1;
}
{% endraw %}
```

That variable `inside` could still be *hoisted* and declared *outside* of the code block by the Javascript engine.

Indeed, even outside of the function!

And, therefore the variable would became exposed and at the same time yet available globally.

Some may think this is a good thing.

However, by extension the now *hoisted* variable also became subject to global corruption, as well.

Hence, the need to contain the scope of the variables declared in ES6.

## ES6 Let

More to come ...

Place the introducing line of text ie.) the 'tagline' here ...

## Import Code

More to come ...

Place the introducing line of text ie.) the 'tagline' here ...

## Last Subtitle

Place the introducing line of text ie.) the 'tagline' here ...

**Note**. The above synopsis was derived from an article written by Blank [[2](#BLANK){:.red}].

### Raw Code Block

```liquid
{% raw %}
Enjoy the successful output!
{% endraw %}
```

{% include patreon-link.md %}.
