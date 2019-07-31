<div>
### Overview

* Intro & History
* Assembly Primer
* Top 5 Optimisations
* Behind the Scenes
* Stop and ask questions! <!-- .element: class="fragment" -->

</div><!-- .element: class="white-bg" -->


<div>
## About me
* Decade of making console games
* Writing C++ tools
* Google, YouTube mobile
* Finance
* But then...<!-- .element: class="fragment" -->
</div><!-- .element: class="white-bg" -->


<div>
## This happened...
![CE logo](images/CE.svg) <!-- .element: class="no-border stretch" -->
</div><!-- .element: class="white-bg" -->


<div>
## Origin Story

* In 2012 I worked in low-latency trading
* "Discussing" c++0x features<!-- .element: class="fragment" -->

```bash
watch "g++ /tmp/test.cc -std=c++0x -O2 -c -S -o - -masm=intel \
    | c++filt \
    | grep -vE '\s+\.'"
```
<!-- .element: class="fragment" -->

</div><!-- .element: class="white-bg" -->


## Live demo!
<!-- .element: class="white-bg" -->


<div>

## Origin Story

* Great
* But not pretty
* TO THE WEB!<!-- .element: class="fragment" -->

</div><!-- .element: class="white-bg" -->


## GCC Explorer!
<!-- .element: class="white-bg" -->
![First version](images/first_working.png)<!-- .element: height="470" class="no-border" -->


<div>

## Evolution
* 2012
  * Colouration & filtering
  * D language support
* 2013
  * Battle hardening
  * More compilers
* 2014
  * goo.gl short links
  * Rust support

</div><!-- .element: class="white-bg" -->


<div>

## Evolution
* 2015
  * Binary support
* 2016
  * GoldenLayout
* 2017
  * Monaco
  * Libraries
</div><!-- .element: class="white-bg" -->


<div>

## Evolution
* 2018
  * Unified languages
  * MS compilers
  * Tools windows
* 2019
  * Bug fixes
  * Cache improvements
  * 6502 support!
</div><!-- .element: class="white-bg" -->


<div>

## Evolution

* Tools:
  * `clang-tidy`
  * `llvm-mca`
  * `pahole`
* Views
  * `opt` output
  * clang AST & IR
  * gcc Tree & IR
  * control flow graph

</div><!-- .element: class="white-bg" -->


## How do _you_ use Compiler Explorer?
<!-- .element: class="white-bg" -->
