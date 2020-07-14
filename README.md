[//]: # (edichokey/readme.md)
[//]: # (2020.7.14)

# edichokey

## Introduction

This is a LaTeX package for typesetting dichotomous identification keys. It can be considered as an extended version of `dichokey`.

## Usage

The usage is almost the same as the package `dichokey`.

~~~latex
\begin{Key}[P.]
\alter Leaves large \name{macrophyllus}
\alter Leaves small.
  \alter Flower solitary.
    \alter Fruits white \name{leucocarpus}
    \alter Fruits black \name{melanocarpus}
  \alter Flowers many \name{pleianthus}
\end{Key}
~~~

## Improvements

* Rewrite core algorithm for complex keys
* Enable dot lines to wrap
* Shift all taxa keyed out right uniformly
 
