<!--
**kevinmonisit/kevinmonisit** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
```bash
Program received signal SIGSEGV, Segmentation fault.
0x00000000004011f4 in read_memory_to_buffer (src_addr=0xffff880000001000, dest_buffer=0x7fffffffd010, size=1024) at memoryops.c:45
45	    memcpy(dest_buffer, (const void *)src_addr, size); // Attempt to copy from protected memory
#0  0x00000000004011f4 in read_memory_to_buffer (src_addr=0xffff880000001000, dest_buffer=0x7fffffffd010, size=1024) at memoryops.c:45
#1  0x000000000040127b in attempt_read_operation () at attempt.c:30
    size_t size = 1024;
    char buffer[size];
    void *readme_addr = (void *)0xffff880000001000;
    read_memory_to_buffer(protected_addr, buffer, sizeof(buffer));
#2  0x000000000040134f in perform_operations () at operations.c:22
    attempt_read_operation();
#3  0x0000000000401432 in initialize_application () at appinit.c:18
    perform_operations();
#4  0x0000000000401520 in main () at main.c:10
    initialize_application();
```
