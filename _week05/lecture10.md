---
title: Some Technical Stuff
layout: lecture
---

## Deduction, Induction, and Our Stories

[play the video, but don't make them watch all of it]

 * What characters are in it?
 * What's the setting?
 * What is the story archetype?

---

## Choosing a Medium

 * Will you be there?
 * How constrained is your story?
 * What technical abilities do you have?
 * How does the data interact?

---

## Technical Choices for a Medium

[Explorables explanations](https://explorabl.es/) has a collection of [tools](https://explorabl.es/tools/) we can explore.

[Kinetic Graphs](https://kineticgraphs.org/) allows you to define specific characteristics, thus enabling mathematical formulas to be manipulated.

[Observable](https://observablehq.com/) is a platform for exploring interactive notebooks, and is particularly well-suited to visualization and design projects.

[GitHub Pages](https://pages.github.com) is a straightforward way of creating HTML (or markdown) and placing it online.  This can include interactivity.

[Glitch](https://glitch.com/) is an environment for exploration of web development and applications which can have server-side components.

---

## Introduction to Javascript and d3

We are going to learn just a *little* bit about Javascript, and then we are going to talk about how we can construct [data-driven documents](https://d3js.org/) by hand.

<p class="fragment">The important thing here isn't what we are building, or the code we write.</p>

<p class="fragment">The important concept is that of binding data to representation.</p>

---

## Javascript in Ten Minutes

You can declare variables in Javascript implicitly or explicitly, depending on
how you want them scoped.

```
var myArray = [1, 2, 3, 4];
var myString = "Hello there!";
var myConcatString = "Hi " + "there " + 5;
var myObject = {'a': 1, 'b': 2, 'c': [1, 2, 3, 4]};
```

---

## Updating variables

If you have an array of objects, there are three very handy functions you can
utilize: `slice`, `forEach` and `filter`.  If you have an object, you can
update it either by accessing a property with a period (`obj.something`) or by
accessing it like you would a dictionary in python (`obj['something']`).

---

## Arrays: `filter`

```
var myArray = [1, 5, 1, 3, 50, 14, 2];
myArrayFiltered = myArray.filter(val => val > 2);
```

Note that here I'm using `=>` as shorthand for declaring a function.

---

## Arrays: `forEach`

To execute something on every value in an array, you can call `forEach` with a
function.

```
var myArray = [1, 2, 3, 4, 5];
myArray.forEach(val => console.log(val * 2));
```

---

## Arrays: `slice`

You can set a start and a stop on an array with a `slice` call:

```
var myArray = ["Hello", "I", "am", "here", "now"];
myArray.slice(3).forEach(word => console.log(word));
```

---

## d3 and Data-Driven Documents

We are now going to try out a little bit -- seriously, not very much at all! -- of [d3](https://d3js.org/).

The best place to try this out is at [ObservableHQ](https://observablehq.com/).

Let's take a look at d3, and then try out some [NEO data](https://data.nasa.gov/resource/2vr3-k9wn.json).
