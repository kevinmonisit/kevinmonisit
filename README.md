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
0x00000000004011f4 in read_readme () at memoryops.c:22
22	    char *readme_addr = (char *)0xffff880000001000; 
#0  0x00000000004011f4 in read_readme () at memoryops.c:22
#1  0x000000000040123a in process_readme_operations () at operations.c:15
#2  0x00000000004012c0 in main () at main.c:25
```
