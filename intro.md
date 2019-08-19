<div>
### Overview

* Intro & History
* Assembly Primer
* Favourite Optimisations
* Behind the Scenes
* Stop and ask questions! <!-- .element: class="fragment" -->

</div><!-- .element: class="white-bg" -->


<div>
## About me
* Decade of making console games
* Writing C++ tools
* Google, YouTube mobile</div><!-- .element: class="white-bg" -->


<div>

## Evolution: 2018

* Finance
* But then...<!-- .element: class="fragment" -->
</div><!-- .element: class="white-bg" -->


<div>
![CE logo](images/CE.svg) <!-- .element: class="no-border stretch" -->
</div><!-- .element: class="white-bg" -->


<div>
## Origin Story

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

## Evolution: 2012-2014
  * Colouration & filtering
  * More compilers
  * D language support
  * Rust support
  * goo.gl short links

</div><!-- .element: class="white-bg" -->


<div>

## Evolution: 2015-2017
  * Binary support
  * GoldenLayout
  * Monaco
  * Libraries
</div><!-- .element: class="white-bg" -->


<div>

## Evolution: 2018
  * Unified languages
  * MS compilers
  * Tools windows

</div><!-- .element: class="white-bg" -->


<div>

## Evolution: 2019
  * 6502 support! <!-- .element: class="fragment" -->
  * Code execution! <!-- .element: class="fragment" -->
  
</div><!-- .element: class="white-bg" -->


<div>

## Evolution: Tools
  * `clang-tidy`
  * `llvm-mca`
  * `pahole`
  * `clang-query`
  * `readelf`
  * `x86-to-6502`

</div><!-- .element: class="white-bg" -->


<div>

## Evolution : Views
  * `opt` output
  * clang AST & IR
  * gcc Tree & IR
  * Control flow graph

</div><!-- .element: class="white-bg" -->
