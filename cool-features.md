<div class="white-bg">

### Compiler Explorer Showcase

</div>

---

<div class="white-bg">

### Simple Example

```cpp
int add(int lhs, int rhs)
{
  int result = lhs + rhs;
  return result;
}
```
<!-- .element: data-ce -->

</div>

---

### Counting Set Bits <!-- .element: class="white-bg" -->

```cpp
int countSetBits(unsigned value) {
  int count = 0;
  while (value != 0) {
    count++;
    value &= (value - 1); // clear lowest set bit
    //       1110100 (value)
    //     - 0000001
    //     = 1110011
    //
    //       1110100 (value)
    //     & 1110011 (value - 1)
    //     = 1100000
  }
  return count;
}
///hide
// notes for Matt...
// * Control Flow Graph
// * march=...
// * llvm opt view
```
<!-- .element: data-ce data-ce-options="-O2 -march=nocona"-->

---

### Sums<!-- .element: class="white-bg" -->

```cpp
int sumOverArray(const int *input, unsigned length) {
///hide
  // if (length & 63 || length == 0)
  //  __builtin_unreachable();
  // or...
  // [[assume((length & 63) == 0 && length > 0)]];

///unhide
  int sum = 0;

  for (unsigned index = 0; index < length; ++index)
    sum += input[index];
  
  return sum;
}
///hide
// notes for Matt...
// * llvm-mca
```
<!-- .element: data-ce data-ce-options="-O3 -march=skylake" --->

---

### LTO

```cpp
/// square.cpp
int square(int x) {
  return x * x;
}

// main.cpp
extern int square(int);

int main() {
  return square(10);
}
```
<!-- .element: data-ce date-ce-options="-O2" -->
