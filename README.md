[//]: # (qdichokey/readme.md)

# qdichokey

## Introduction

This is a LaTeX package for TeXnical taxonomists to make dichotomous identification keys.

## Usage

The usage is similar to the package `dichokey`, except for the asterisked name of environment `Key*`.

~~~latex
\begin{Key*}{A.~} % Acronym for an anonymous genus
\alter Leaves large \name{macrophyllum}
\alter Leaves small.
	\alter Flowers large.
		\alter Capsules large \name{macrospermum}
		\alter Capsules small \name{microspermum}
	\alter Flowers small \name{microflorum}
\end{Key*}
~~~

## Improvements

* Rewrite core algorithm for large keys with more than 31 terminal taxa
* Make dot lines line-breakable
* Shift all taxa keyed out right uniformly
 
## Update History

- 2017.12.13: ver. 2, released on Github

## Caution

Incompatible with the `adjustwidth` environment in package `changepage`, since the `\parshape` command is reloaded.

## 一些有的没的

原来想着 `dichokey` 宏包改改用，但在排 *Flora of China* 的葱属分种检索表时炸了，原因是该宏包用一个计数器的二进制位来储存分枝序号对的状态，因而检索表规模受到整型字长的限制，最多只能有 30 对分枝，换言之最多 31 个分类阶元。于是重写一个。

