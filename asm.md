## Assembly!
<!-- .element: class="white-bg" -->

<div class="fragment white-bg">
<img src="images/One_Ring_inscription.svg" height="200" class="no-border">
<div class="attribution">
<a href="https://commons.wikimedia.org/wiki/User:Ssolbergj">Ssolbergj</a>, Wikimedia Commons CC SA 4.0
</div>
<aside class="notes">
Ash nazg durbatulûk, ash nazg gimbatul,
Ash nazg thrakatulûk agh burzum-ishi krimpatul.
</aside>
</div>


### x86-64 Assembly
<!--- .element: class="white-bg" -->

```x86asm
  instr
  instr dest_operand
  instr dest_operand, source_operand
  instr dest_operand, source_operand, source_operand
```

```x86asm
  ret                           ; return
  inc rax                       ; increment "rax"
  mov edx, 1234                 ; set "edx" to the value 1234 
  add rsi, rdi                  ; "rsi" += "rdi" 
  vpaddd ymm1, ymm2, ymm0       ; "ymm1" = "ymm2" + "ymm0"
```
<!-- .element: class="fragment" -->


### Instructions
<!--- .element: class="white-bg" -->

<div class="w30 white-bg"><ul class="instr fragment highlight-current-red">
<li><code>mov</code></li>
<li><code>movzx</code></li>
<li><code>movsxd</code></li>
<li><code>lea</code></li>
</ul><ul class="instr fragment highlight-current-red">
<li><code>call</code></li>
<li><code>ret</code></li>
<li><code>jmp</code></li>
</ul></div>

<div class="w30 white-bg"><ul class="instr fragment highlight-current-red">
<li><code>push</code></li>
<li><code>pop</code></li>
</ul><ul class="instr fragment highlight-current-red">
<li><code>cmp</code></li>
<li><code>test</code></li>
<li><code>je</code></li>
<li><code>jne</code></li>
</ul></div>

<div class="w30 white-bg"><ul class="instr fragment highlight-current-red">
<li><code>and</code></li>
<li><code>xor</code></li>
<li><code>add</code></li>
<li><code>sub</code></li>
<li><code>shl</code></li>
<li><code>shr</code></li>
<li><code>sar</code></li>
</ul></div>

<div><br><br></div>

<div class="fragment white-bg">
And many, many more...
</div>


### Operands
<!--- .element: class="white-bg" -->

```x86asm
  register                          ; e.g. rax, rbx, ecx...
  constant                          ; e.g. 1234
  <size> ptr [register]             ; e.g. DWORD PTR [rax]
  <size> ptr [register + offset]    ; e.g. BYTE PTR [rcd + rsi]
  <size> ptr [register + offset + register2 * (1,2,4,8)]
```

```x86asm
  add eax, dword ptr [rdi + 12 + rsi * 4] 
                                ; eax += *(int *)(rdi + 12 + rsi * 4)
```
<!-- .element: class="fragment" -->


### Registers
<!--- .element: class="white-bg" -->

<div class="white-bg">
<ul>
<li><code>rax</code> (return value)</li> 
<li><code>rdi</code> (1st param)</li> 
<li><code>rsi</code> (2nd param)</li> 
<li><code>rdx</code> (3rd param)</li>
<li><code>rbx</code> <code>rcx</code> <code>rbp</code> <code>r8-r15</code> <code>rsp</code></li>
<li><code>xmm0-15</code> (<code>ymm0-15</code>... <code>zmm0-31</code>... <code>k0-7</code>)</li>
</ul></div>


<table class="registers white-bg">
    <thead>
    <tr>
        <th>63...56</th>
        <th>55...48</th>
        <th>47...40</th>
        <th>39...32</th>
        <th>31...24</th>
        <th>23...16</th>
        <th>15...8</th>
        <th>7...0</th>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td colspan="8" class="register rax">rax</td>
    </tr>
    <tr>
        <td colspan="4" class="regnote">(zeroed on write)</td>
        <td colspan="4" class="register eax">eax</td>
    </tr>
    <tr>
        <td colspan="6"></td>
        <td colspan="2" class="register ax">ax</td>
    </tr>
    <tr>
        <td colspan="6"></td>
        <td colspan="1" class="register ah">ah</td>
        <td colspan="1"></td>
    </tr>
    <tr>
        <td colspan="7"></td>
        <td colspan="1" class="register al">al</td>
    </tr>
    </tbody>
</table>


<!-- .slide: data-background="./images/bg/weave.jpg" -->
## Important note on performance
<!-- .element: class="white-bg" -->

<div class="fragment white-bg">
<ul>
<li><a href="https://github.com/google/benchmark">Google Benchmark</a></li>
<li><a href="https://github.com/nickbruun/hayai">hayai</a></li>
<li><a href="https://github.com/rmartinho/nonius">Nonius</a></li>
<li><a href="http://quick-bench.com/">Quick Bench</a></li>
</ul>
</div>
