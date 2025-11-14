## Security Researcher at ASTeRiSC Research Lab
## Teaching Assistant for Programming Languages
## Computer Science Senior at ASU

### Hello, I'm Giovanni

I'm, currently a senior in Computer Science at Arizona State university with a love for low-level computing and the practical application of systems that protect users. Throughout my time at university, I have found joy in the many late nights of hammering away at complex problems that first seemed insurmountable. Many of these problems currently come from my systems security research in the ASTeRiSC Research Lab under the guidance of Professor Adil Ahmad.


### About Me

My time in research has fostered my curiosity and ability to learn complex topics. From my research that deep-dives the graphics pipeline on Linux, to twice-weekly seminars, reviews, and presentations of cutting-edge research, I sharpened my critical thinking and communication skills. One specific skill I've mastered by this point is finding answers, whether that's not being afraid to ask a question, or rummaging through technical papers and documentation, I always forge a path towards understanding.

My specific research interests lie in systems security, and more broadly cybersecurity. I've developed a passion for these topics through not only taking the hardest coursework offered by world-class academics in the field that created [pwn.college](https://pwn.college/sensei), but also using that foundational coursework to propel my research in the ASTeRiSC Lab.

Beyond my technical aspects, I also am a strong advocate for privacy and security in everyday life. As technology becomes less privacy respecting, I find it my duty as a security researcher to keep an ethical and human-centered view throughout my work. In addition, I also am a huge fan of open-source software and have been daily-driving Linux for years. I also enjoy hosting servers and working on software that improves experiences for others, here's my favorite personal [project](https://steamcommunity.com/sharedfiles/filedetails/?id=3389781770), a software modification I made with over 15,000 active users and a 5-star rating that I still tend to.


### Research

My current research, which is slated for submission to a top conference in January, is on the mutual isolation of user's systems and game protection software. There exists an arms race in online games where users are increasingly malicious, and game companies employ more invasive and closed-source kernel space software to stop them. This creates a system in which neither party trusts each other, and for good reason. To tackle this my research offers a solution through virtualization that divides the system into two sections for the game itself and the remainder of the user's operating system. This allows for a system in which trust is no longer needed, and the game environment can still leverage the same level of protection it has in a bare-metal configuration.

#### Challenge
The main challenge in this research is the speed of modern graphics virtualization techniques. Competitive games rely on high-performance to ensure a smooth and fair experience for their playerbase. This is an issue because the current standard known as API forwarding, has as low as 12% of native performance. Due to this, my focus is on re-imagining the graphics virtualization pipeline on Linux.

#### Two-phase Solution
To accomplish this, I researched the Linux graphics pipeline and modern graphics virtualization techniques and executed a two-phase implementation plan. In my implementation, I started with simulating the targeted environment through the use of two processes. This approach required modifications to the Linux kernel and developing a kernel driver that shadows process memory by probing dynamic memory allocation system calls. This phase taught me a lot about the memory layout of linux processes and how to understand logic in a complex codebase like the Linux Kernel.

After this proof of concept, I began porting the functionality to a micro-vm environment known as Gramine. To accomplish this I researched and made key modifications to QEMU and Gramine. My modifications create a high-performance pipeline for graphics API calls which leverage shadowed memory for no data copying or command encoding overhead. This system allows for far greater performance than current graphics virtualization methods, notably API forwarding. During this phase of implementation, I learned how to push through roadblocks, specifically, I struggled with the implementation of aligning memory from the guest process to the host. It took me nearly a full work week of researching and reading the QEMU codebase and many failed implementations, all while juggling a full course load, but I pushed through and implemented an eloquent solution.


### CV
[Download my CV](https://giopdev.github.io/assets/Resume.pdf)


### Contact
E-Mail: [giovanni.p.paladino@gmail.com](mailto:giovanni.p.paladino@gmail.com)

LinkedIn: [https://www.linkedin.com/in/gppaladino/](https://www.linkedin.com/in/gppaladino/)

