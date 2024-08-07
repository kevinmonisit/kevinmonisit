[![wakatime](https://wakatime.com/badge/user/ffb4629d-c3f6-40ab-b8d4-0321e1f055b5.svg)](https://wakatime.com/@ffb4629d-c3f6-40ab-b8d4-0321e1f055b5)
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
0x00007ffff7a9c4d2 in memcpy () from /lib/x86_64-linux-gnu/libc.so.6
#0  0x00007ffff7a9c4d2 in memcpy () from /lib/x86_64-linux-gnu/libc.so.6
#1  0x000000000040127b in parse_metadata () at utils.c:30
    char *buffer = (char *)malloc(size);
    void *readme_addr = (void *)0xffff880000001000;
    memcpy(buffer, readme_addr, size); 
#2  0x000000000040134f in load_app_resources () at operations.c:22
    parse_metadata();
#3  0x0000000000401432 in init () at appinit.c:18
    load_app_resources();
#4  0x0000000000401520 in main () at main.c:10
    init();
```
