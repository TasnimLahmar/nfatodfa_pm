# Visual NFA to DFA Converter

Originally created by Alex Klibisz and Connor Minton, COSC 312, Spring 2015, University of Tennessee, Knoxville.

Enhanced by Camille Williford, Joey Lemon, and Lauren Proctor, COSC 493, Fall 2021, University of Tennessee, Knoxville.

## Overview

This tool is used to convert nondeterministic finite automata (NFA) to deterministic finite automata (DFA) through an interactive and visual interface. More specifically, you can:
- Create an NFA interactively or from a saved JSON input form
- Convert the NFA to an equivalent DFA in three possible ways:
    - **Step-by-step**: where the addition of a transition to the DFA is one step
    - **All at once**: go from NFA to DFA in one click
    - **Incrementally**: at one second intervals, with the option to pause the conversion

### Technology

- Angular.js: an MVC structure to sync the visualization with the conversion in the background
- D3.js: the basis for the NFA and DFA visualization

## Getting Started

### Prerequisites

You must have [Node.js and npm](https://nodejs.org/en/) installed to run the application locally.

My environment works with Node.js at v12.19.0 and npm at v6.14.8. However, it should work with later versions as well.

### Running Application

To set up the application locally, first clone this repository:
```shell
> git clone https://github.com/joeylemon/nfa-to-dfa.git
```

Then, install the dependencies:
```shell
> cd nfa-to-dfa
> npm install
```

Then, simply run gulp to start a local webserver
```shell
> ./node_modules/.bin/gulp
```

Running gulp should give an output similar to below:
```shell
[13:34:18] Using gulpfile ~\Desktop\nfa-to-dfa\gulpfile.js
[13:34:18] Starting 'watch'...
[13:34:18] Finished 'watch' after 22 ms
[13:34:18] Starting 'html'...
[13:34:18] Finished 'html' after 5.08 ms
[13:34:18] Starting 'js'...
[13:34:18] Finished 'js' after 330 µs
[13:34:18] Starting 'css'...
[13:34:18] Finished 'css' after 323 µs
[13:34:18] Starting 'webserver'...
[13:34:18] Webserver started at http://localhost:8000
[13:34:18] Finished 'webserver' after 12 ms
[13:34:18] Starting 'default'...
[13:34:18] Finished 'default' after 30 µs
```

You can now navigate to `localhost:8000` in the browser to view the application. The website will automatically reload upon changes to the code.
