```C
int main(void) 
{
  int n = 50;
  int *p = &n;
  printf("%p", p)  // %p to print the pointer value: 0x7ffcb4578e5c ~ 8 byte
  printf("%p", &n) // &n is the address of n, same value as p
  printf("%i", *p); // go to address of p and get value: 50
}
```
**p** is the pointer that holds the memory address of another variable, it's n in this case.
***p** in printf means de-reference of p, and get value that stored in that address
