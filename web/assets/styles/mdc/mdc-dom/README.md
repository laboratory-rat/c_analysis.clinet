<!--docs:
title: "DOM"
layout: detail
section: components
excerpt: "Provides commonly-used utilities for inspecting, traversing, and manipulating the DOM."
path: /catalog/dom/
-->

# DOM

MDC DOM provides commonly-used utilities for inspecting, traversing, and manipulating the DOM.

Most of the time, you shouldn't need to depend on `mdc-dom` directly. It is useful however if you'd like to write custom components that follow MDC Web's pattern and elegantly integrate with the MDC Web ecosystem.

## Installation

```
npm install ../mdc-dom
```

## Basic Usage

```js
import * as ponyfill from '../mdc-dom/ponyfill';
```

> See [Importing the JS component](../../docs/importing-js.md) for more information on how to import JavaScript.

## Ponyfill Functions

The `ponyfill` module provides the following functions:

Function Signature | Description
--- | ---
`closest(element: Element, selector: string) => ?Element` | Returns the ancestor of the given element matching the given selector (which may be the element itself if it matches), or `null` if no matching ancestor is found.
`matches(element: Element, selector: string) => boolean` | Returns true if the given element matches the given CSS selector.
