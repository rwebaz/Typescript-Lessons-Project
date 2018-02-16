---
title: ES5 Variables
layout: default
excerpt: Place the introducing line of text ie.) the 'lead' here ...
version: Page Template md Dtd 02-15-18
navigation_weight: 8
categories: es5
---
# {{ page.title }}

{{ page.excerpt }}

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

## Import Code

More to come ...

## Last Subtitle

**Note**. The above synopsis was derived from an article written by Blank [[2](#BLANK){:.red}].

### Raw Code Block

```liquid
{% raw %}
Enjoy the successful output!
{% endraw %}
```

{% include brackets-ide.md %}

{% include sources-and-uses.md %}

### External Sources

- {:#SOURCELINKS}The [Project Source Links](https://mminail.github.io/Typescript/Source-Typescript-Links.htm){:title='Click to Visit the Source Links page of the Typescript Lessons Project at Concepts Library'}{:target='_blank'} page of the Typescript Lessons Project at Concepts Library. Published by © 2017 - 2018 [Mminail.github.io](https://mminail.github.io/){:title='Click to Visit the Home Page of the Concepts Library of the Medical Marijuana Initiative of North America - International Limited, an Arizona Benefit Corporation'}{:target='_blank'}.

**Note**. This page crafted with {{ page.version }}.
