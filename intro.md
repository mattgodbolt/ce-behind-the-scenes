<div class="white-bg">

### Overview
* Intro & History
* Behind the Scenes
* ASM primer
* Lesser-known Features
* Cool Optimizations

</div>

---
    
<div class="white-bg">

### About me

* Decade of making console games
* Writing C++ tools
* Google, YouTube mobile
* Finance
* But then...<!-- .element: class="fragment" -->

</div>

---

<div class="white-bg">

![CE logo](images/CE.svg) <!-- .element: class="no-border stretch" -->

</div>

---

<div class="white-bg">

### Compiler Explorer?

* [godbolt.org](https://godbolt.org/z/BcrSDt)
* Why is it useful?
* How it it used?

</div>

---

<div class="white-bg">

### Origin Story

```bash
watch "g++ /tmp/test.cc -std=c++0x -O2 -c -S -o - -masm=intel \
    | c++filt \
    | grep -vE '\s+\.'"
```
<!-- .element: class="fragment" -->

</div>

---

<img src="images/ce-sh.png" width="2560" height="1440" style="height: 500px; width: auto;">

---

<div class="white-bg">

## Origin Story

* Great
* But not pretty
* TO THE WEB!<!-- .element: class="fragment" -->

</div>

---

### GCC Explorer!
<!-- .element: class="white-bg" -->
![First version](images/first_working.png)<!-- .element: height="470" class="no-border" -->
