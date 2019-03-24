## Best 5 Compiler Optimisations
<!-- .element: class="white-bg" -->

```cpp
int countSetBits(unsigned a)
{
  int count = 0;
  while (a != 0)
  {
    count++;
    // clear bottom set bit
    a &= (a - 1);
  }
  return count;
}
```


```cpp
bool isspc(char c)
{
  return c == ' '
    || c == '\r'
    || c == '\n'
    || c == '\t';
}
```


```x86asm
  movabs rax, 0x100002600  ; 0b100000000000000000010011000000000
                           ;   ^                  ^  ^^
                           ;   +- bit 32          |  ++- b10 & 9
                           ;              bit 13 -+
  shrx rax, rax, rdi       ; shift right 'rdi' times
  and eax, 1               ; pick the lowest set bit
```


```cpp

int sumToX(int x)
{
  int result = 0;
  for (int i = 0; i < x; ++i)
  {
    result += i;
  }
  return result;
}
```


```cpp
unsigned divideXbyY(unsigned x, unsigned y)
{
  return x / y;
}
```
