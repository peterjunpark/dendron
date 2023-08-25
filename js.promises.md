---
id: zvb67ed54dr1eggtsbt5vud
title: Promises
desc: ""
updated: 1692510659969
created: 1692510393729
---

## Promise.all()

The `Promise.all()` static method takes an iterable of promises as input and returns a single Promise. This returned promise fulfills when all of the input's promises fulfill (including when an empty iterable is passed), with an array of the fulfillment values. It rejects when any of the input's promises rejects, with the first rejection reason.

## Promise.resolve()

The `Promise.resolve()` static method _resolves_ a given value given to a Promise. If the value is a promise, that promise is returned; if the value is a **thenable**, `Promise.resolve()` will call the `then()` method with two callbacks it prepared; otherwise the returned promise will be fulfilled with the value.
