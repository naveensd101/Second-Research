```c 
union datapacket {
	int data;
	char mem[4]; //4 bytes = 4*8 = 32 bits, which is size of data
};
```

[[Murali sir]]

**Murali sir is awesome**

The whole USP is that if the data is stored in big endian format, we can easily convert it to little endien by reversing the mem array.
Since we are using union both these variables represend the same area in the memory

---

More hacks like this are available in ![[misurda.pdf]]