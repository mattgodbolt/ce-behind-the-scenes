<div class="white-bg">

### Unified languages

[Link](http://localhost:10240/#g:!((g:!((g:!((h:codeEditor,i:(fontScale:2.2290251120639994,j:1,lang:rust,source:'//+Type+your+code+here,+or+load+an+example.%0Apub+fn+square(num:+i32)+-%3E+i32+%7B%0A++++num+*+num%0A%7D%0A'),l:'5',n:'0',o:'Rust+source+%231',t:'0')),k:50,l:'4',n:'0',o:'',s:0,t:'0'),(g:!((h:compiler,i:(compiler:r1330,filters:(b:'0',binary:'1',commentOnly:'0',demangle:'0',directives:'0',execute:'1',intel:'0',libraryCode:'1',trim:'1'),fontScale:2.2290251120639994,lang:rust,libs:!(),options:'-O',source:1),l:'5',n:'0',o:'rustc+1.33.0+(Editor+%231,+Compiler+%231)+Rust',t:'0')),k:50,l:'4',n:'0',o:'',s:0,t:'0')),l:'2',n:'0',o:'',t:'0')),version:4)

<aside class="notes">

* Show rust
* Bring up C++
* Show diff

</aside>

</div>

---
<div class="white-bg">

### Tools & Views

[Link](http://localhost:10240/#g:!((g:!((g:!((h:codeEditor,i:(fontScale:2.23,j:1,lang:c%2B%2B,source:'int+sumOverArray(const+int+*input,+unsigned+length)+%7B%0A++input+%3D+static_cast%3Cconst+int+*%3E(%0A++++++__builtin_assume_aligned(input,+64))%3B%0A++if+(length+%26+63+%7C%7C+length+%3D%3D+0)+%7B%0A++++__builtin_unreachable()%3B%0A++%7D%0A%0A++int+sum+%3D+0%3B%0A++for+(int+i+%3D+0%3B+i+%3C+length%3B+%2B%2Bi)+%7B%0A++++sum+%2B%3D+input%5Bi%5D%3B%0A++%7D%0A++%0A++return+sum%3B%0A%7D%0A'),l:'5',n:'0',o:'C%2B%2B+source+%231',t:'0')),k:50,l:'4',n:'0',o:'',s:0,t:'0'),(g:!((h:compiler,i:(compiler:g91,filters:(b:'0',binary:'1',commentOnly:'0',demangle:'0',directives:'0',execute:'1',intel:'0',libraryCode:'1',trim:'1'),fontScale:2.23,lang:c%2B%2B,libs:!(),options:'-march%3Dhaswell+-O3',source:1),l:'5',n:'0',o:'x86-64+gcc+9.1+(Editor+%231,+Compiler+%231)+C%2B%2B',t:'0')),k:50,l:'4',n:'0',o:'',s:0,t:'0')),l:'2',n:'0',o:'',t:'0')),version:4)

[Link](http://localhost:10240/#g:!((g:!((g:!((g:!((h:codeEditor,i:(fontScale:2.23,j:1,lang:c%2B%2B,source:'int+sumOverArray(const+int+*input,+unsigned+length)+%7B%0A++input+%3D+static_cast%3Cconst+int+*%3E(%0A++++++__builtin_assume_aligned(input,+64))%3B%0A++if+(length+%26+63+%7C%7C+length+%3D%3D+0)+%7B%0A++++__builtin_unreachable()%3B%0A++%7D%0A%0A++int+sum+%3D+0%3B%0A++for+(int+i+%3D+0%3B+i+%3C+length%3B+%2B%2Bi)+%7B%0A++++sum+%2B%3D+input%5Bi%5D%3B%0A++%7D%0A%0A++return+sum%3B%0A%7D%0A'),l:'5',n:'0',o:'C%2B%2B+source+%231',t:'0')),k:50,l:'4',m:50,n:'0',o:'',s:0,t:'0'),(g:!((h:codeEditor,i:(fontScale:2.23,j:2,lang:analysis,source:'++++++++vpaddd++ymm0,+ymm0,+YMMWORD+PTR+%5Brdi%5D%0A++++++++add+++++rdi,+32%0A++++++++cmp+++++rax,+rdi%0A++++++++jne+++++.L2%0A'),l:'5',n:'0',o:'Analysis+source+%232',t:'0')),header:(),l:'4',m:50,n:'0',o:'',s:0,t:'0')),k:62.5,l:'3',n:'0',o:'',t:'0'),(g:!((g:!((h:compiler,i:(compiler:g91,filters:(b:'0',binary:'1',commentOnly:'0',demangle:'0',directives:'0',execute:'1',intel:'0',libraryCode:'1',trim:'1'),fontScale:2.23,lang:c%2B%2B,libs:!(),options:'-march%3Dhaswell+-O3',source:1),l:'5',n:'0',o:'x86-64+gcc+9.1+(Editor+%231,+Compiler+%231)+C%2B%2B',t:'0')),k:37.5,l:'4',m:50,n:'0',o:'',s:0,t:'0'),(g:!((h:compiler,i:(compiler:llvm-mcatrunk,filters:(b:'0',binary:'1',commentOnly:'0',demangle:'0',directives:'0',execute:'1',intel:'0',libraryCode:'1',trim:'1'),fontScale:2.23,lang:analysis,libs:!(),options:'-mcpu%3Dhaswell+-timeline+-iterations%3D10',source:2),l:'5',n:'0',o:'llvm-mca+(trunk)+(Editor+%232,+Compiler+%232)+Analysis',t:'0')),header:(),l:'4',m:50,n:'0',o:'',s:0,t:'0')),k:37.5,l:'3',n:'0',o:'',t:'0')),l:'2',m:100,n:'0',o:'',t:'0')),version:4)

</div>

---

<div class="white-bg">

* pahole
* readelf
* clang-query
* x86-to-6502
* CFG
* `#include <http://...>`
* Compiler viewers (RTL/LLVM IR/Parse)

</div>
