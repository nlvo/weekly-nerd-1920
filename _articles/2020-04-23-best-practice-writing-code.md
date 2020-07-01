---
layout: post
title:  "👍 Best practice writing code"
date:   2020-04-23 10:56:44 +0200
categories: articles
---
While following the web minor, I've been interested in how to write clean and easy to read code but also the structure itself. I'll be writing not only about what I've read but also about my findings.

- Functional programming
- Make it work..then beautiful and last but not least make it fast

## Functional programming

What is [functional programming](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-functional-programming-7f218c68b3a0)?

> Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data — Wikipedia

A couple of concepts for [functional programming](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-functional-programming-7f218c68b3a0) are:

- Pure functions
- Function composition
- Avoid shared state
- Avoid mutating state
- Avoid side effects

The idea is that every function has it's own purpose which makes it easier to debug and understand from an outsiders perspective. It's also supposed to be easier to read.

The two concepts I focused on were, pure functions and the side effects. Pure functions are functions who do just one thing and have no side effects.

> Side-effect is any external effect a function has besides its return value — [Eric Normand](https://lispcast.com/what-are-side-effects/).

This is something I've tried to practice within the minor as much as possible, while I can't say that I've mastered it in any way. I do however believe it has helped a lot in order to keep my code clean.

*This is an example from a project I made while trying this concept out. It's based of on an example given by Guido.*

{% highlight javascript %}
// get all the comics and return the data
async function getAll () {
	const charactersEndpoint = createCharactersEndpoint();
	const characters = await fetch(charactersEndpoint);
	return characters;
}
{% endhighlight %}

Benefits I've personally found, there are probably way more benefits, but these are the ones I've found.. while trying this concept for the first time

- easy to debug
- clean
- reusable

## Make it work..then beautiful and last but not least make it fast - Guido

The first thing you usually do is figure out what the problem is, which you then try to solve. And if you have time left you try to make it better etc.

- work
- beautiful
- fast

This is something that has stuck with me, because it's something I think we all do to a certain degree but never really think about.

Overall it may not seem like a lot, but every little bit help. And I'm less terrified to read my old code, as a matter of fact I actually worked on the same code from Web app from scratch till Progressive Web App. Which was a lot of fun, because you could see the code grow little by little. And it's still readable, if I say so myself. Say no to spaghetti code!