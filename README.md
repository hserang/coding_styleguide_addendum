# Coding Styleguide Addendum
*a companion to your existing style guide*

## Table of Contents
1. [Purpose](#purpose)
1. [Audience](#audience)
1. [Guiding Principles](#guiding-principles)

## Purpose of this doc
<a name="purpose"></a><a name="1.1"></a>
This doc intends to codify some guiding principles of writing code which are not easily detected or enforced by a linter. As there are already many great styleguides in circulation, this is meant to augment those rather than creating another exhaustive list.

## Intended audience
<a name="audience"></a><a name="1.2"></a>
The intended audience for this doc is coders, collaborators and teams. The primary target language is JS/ES/TS but the concepts can apply to other languages.

## Guiding Principles
<a name="guiding-principles"></a><a name="1.3"></a>
* Create code with clarity and empathy in mind
* Be empathetic to your colleagues; Your future self is a colleague whom you haven't yet met

## Code is documentation
<a name="code-documentation"></a><a name="1.4"></a>
*Code is both a document of intent as well as an instruction set of execution*
* Declaritive over imperative
```javascript
// yes
if (isWithinValidRange(someValue)) {
    doSomthing();
} 

// no
if (someValue && someValue <= 5 || someValue > 125) {
    doSomthing();
} 
```
* All function names are descriptive and verb-based
```javascript
// yes
const isValidPhoneNumber = (number) => ...

// no
const phoneNumber = (number) => ...

// yes
const getUsernameById = (id) => ...

// no
const userName = (id) =>
```

* No magic strings/numbers
```javascript
// yes
const PI = 3.14;
const getAreaFromRadius = radius => PI * radius ^ 2;

// no
const getAreaFromRadius = radius => 3.14 * radius ^ 2;

```

* Favor code clarity over terseness in both names a patterns
* Consistency over innovation (unless new innovation becomes the consistency).


