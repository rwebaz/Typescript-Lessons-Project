---
title: Access Modifiers
layout: default
excerpt: Modifiers that define how an interaction may access the properties and methods of a `class` are called `Access Modifiers` in Typescript ...
description: By default, all properties of a `class` and all methods of a `class` are exposed publicly in Typescript unless otherwise modifed by an `Access Modifier` in Typescript.
repo: Typescript-Lessons-Project 
ver_date: 11-17-19
navigation_weight: 8
categories: page
---
{% include toc.md %}

## Public O Private

{{ page.description}}

By default, all properties of a Class and all methods of a Class are exposed publicly.

A *public* exposure in Typescript grants access to all parties in any combination of interactions that are possible to be performed.

**Note.** The *public* access feature in Typescript is also available to any external caller unless modified by the programmer.

### Private Lockdown

In order to *ungrant* the default **public** access in Typescript, all properties and methods of the Class must explicitly be tagged as **private** with the keyword of `private`, as follows:

```typescript
{% raw %}
private var y = x.charAt(6);
{% endraw %}
```

**Note**. The keyword of `public` is also reserved for those moments of coding where the developer wishes to make explicit the already implicit feature of Typescript's default **public** access.

### Protected Methods

A simple extension of a Class into a *child* class is not sufficient to award access to `private` methods of the *parent* class.

For that, the *protected* access modifier keyword is essential.

The `protected` keyword can be placed in front of a *parent* Class method or property statement, as follows:


```typescript
{% raw %}
protected var y = x.charAt(6);
{% endraw %}
```

The *protected* access modifier through the application of the `protected` keyword allows permission for a *child* class to view the properties of its *parent* class.

In addition, by applying the keyword `protected` to a method declared in the parent class any *child* functions may call the methods of the *parent* Class so tagged, as well.

## Read Only Properties

If we take the same *parent* class property as shown above and assign the `readonly` keyword to the property statement, then the risk of a *mutated* value from a collision outside or from inside of the Class from another *child* or *alien* class attempting modification of the value is eliminated.

In effect, the `readonly` keyword creates a modified access to the property that will allow for the view and usage from within the *parent* Class, but retains immutability from without, as follows:

```typescript
{% raw %}
readonly var y = x.charAt(6);
{% endraw %}
```

**Note**. Access modifier keywords may be combined to produce more robust forms of delegation.

For example, prefixing the `private` keyword to the `readonly` keyword creates a variable that can only be viewed from within the *parent* Class, as follows:

```typescript
{% raw %}
private readonly var y = x.charAt(6);
{% endraw %}
```

## Last Subtitle

Place the introducing line of text ie.) the 'tagline' here ...

**Note**. The above synopsis was derived from an article written by Blank [[2](#BLANK){:.red}].

### Raw Code Block

```liquid
{% raw %}
Enjoy the successful output!
{% endraw %}
```

{% include patreon-link.md %}
