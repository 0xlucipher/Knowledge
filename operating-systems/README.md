# Operating systems

I love using [macOS](../macos/) as my personal OS.

And I like [NixOS](linux/nixos.md) and it's [nix package manager](../package-managers/nix/).

## Interesting OSes

* [MirageOS](https://github.com/mirage/mirage) - Library operating system that constructs unikernels.
* [QubesOS](https://www.qubes-os.org/)
* [Plan 9](https://9p.io/plan9/)
* [Toddler](https://github.com/zhengruohuang/toddler) - Well-designed usable and portable microkernel OS.
* [OS67](https://github.com/SilverRainZ/OS67) - Unix-like toy kernel.
* [Serenity](https://github.com/awesomekling/serenity) - X86 Unix-like operating system for IBM PC-compatibles.
* [Resea](https://github.com/seiyanuta/resea) - Pure microkernel-based hackable operating system written from scratch in C and Rust.
* [Rux](https://github.com/sorpaas/rux) - Hobbyist microkernel written in Rust, featuring a capability-based system similar to seL4.
* [redshirt](https://github.com/tomaka/redshirt) - Experiment to build some kind of operating-system-like environment where executables are all in WASM and are loaded from an IPFS-like decentralized network.
* [Spectrum](https://spectrum-os.org/) - Step towards usable secure computing. \([Developer manual](https://spectrum-os.org/doc/developer-manual.html)\) \([Discussions](https://spectrum-os.org/lists/hyperkitty/list/discuss@spectrum-os.org/)\)
* [mikado](https://github.com/cavedweller/mikado) - RISC-V Experimental OS.
* [mkernel](https://github.com/arjun024/mkernel) - Minimalist kernel which prints "my first kernel" on the screen and then hangs. \([HN](https://news.ycombinator.com/item?id=22087701)\)
* [Barebones](https://github.com/fwsGonzo/barebones) - Barebones multiboot kernel for beginners.
* [xv6](https://github.com/mit-pdos/xv6-public) - Re-implementation of Dennis Ritchie's and Ken Thompson's Unix Version 6. \([Paper](https://pdos.csail.mit.edu/6.828/2019/xv6/book-riscv-rev0.pdf)\) \([HN](https://news.ycombinator.com/item?id=22511569)\)
* [xv6 for RISC-V](https://github.com/mit-pdos/xv6-riscv)
* [Orange Slice](https://github.com/gamozolabs/orange_slice) - Research kernel and hypervisor attempting to get fully deterministic emulation with minimum performance cost.
* [Cloud Hypervisor](https://github.com/cloud-hypervisor/cloud-hypervisor) - Open source Virtual Machine Monitor \(VMM\) that runs on top of KVM.
* [RancherOS](https://github.com/rancher/os) - Tiny Linux distro that runs the entire OS as Docker containers.
* [Bottlerocket OS](https://github.com/bottlerocket-os/bottlerocket) - Free and open-source Linux-based operating system meant for hosting containers.
* [XNU kernel](https://github.com/apple/darwin-xnu) - Part of the Darwin operating system for use in macOS and iOS operating systems.
* [Haiku](https://github.com/haiku/haiku) - Open-source operating system that specifically targets personal computing. \([HN](https://news.ycombinator.com/item?id=23469209)\)
* [Pebble](https://github.com/IsaacWoods/pebble) - Microkernel and userspace written in Rust, with first-class message passing.
* [seL4 microkernel](https://github.com/seL4/seL4) \([Article](https://microkerneldude.wordpress.com/2020/04/07/the-sel4-foundation-what-and-why/)\) \([HN](https://news.ycombinator.com/item?id=22801864)\)
* [Barebones amd64 kernel built using 9front](https://github.com/majiru/barebones9)
* [RustyHermit](https://github.com/hermitcore/libhermit-rs) - Rust-based, lightweight unikernel.
* [Distaff](https://github.com/GuildOfWeavers/distaff) - Zero-knowledge virtual machine written in Rust.
* [zCore](https://github.com/rcore-os/zCore) - Reimplement Zircon microkernel in Rust.
* [9front](http://9front.org/) \([Lobsters](https://lobste.rs/s/n5zmtt/9front_plan9_haters_released)\)
* [lilith](https://github.com/ffwff/lilith) - POSIX-like x86-64 kernel and userspace written in Crystal.
* [Genode](https://genode.org/index) - Operating System Framework.
* [Shrine](https://github.com/minexew/Shrine) - TempleOS distro for heretics.
* [Subgraph OS](https://subgraph.com/) - Desktop computing and communications platform that is designed to be resistant to network-borne exploit and malware attacks. \([Handbook](https://github.com/subgraph/sgos_handbook)\)
* [Mezzano](https://github.com/froggey/Mezzano) - Operating system written in Common Lisp.
* [Collapse OS](https://github.com/hsoft/collapseos) - Bootstrap post-collapse technology. \([HN](https://news.ycombinator.com/item?id=21182628)\)
* [LegoOS](https://github.com/WukLab/LegoOS) - Disseminated, Distributed OS for Hardware Resource Disaggregation.
* [CuBitOS](https://github.com/docandrew/CuBit) - General-purpose, formally-verified, 64-bit operating system in SPARK/Ada for x86-64.
* [Demikernel](https://github.com/demikernel/demikernel) - Library operating system architecture designed for use with kernel-bypass I/O devices.
* [Drone](https://www.drone-os.com/) - Embedded Operating System for writing real-time applications in Rust. \([drone-core](https://github.com/drone-os/drone-core)\)

## Notes

* [kernels are virtual machines and we write far better systems when we’re aware of what the VM underneath our programs is going to do to translate our use of memory, files, sockets and threads into things that happen in hardware](https://lobste.rs/s/x1kzuw/what_tools_made_you_better_programmer)

## Links

* [Introduction to Operating Systems](http://pages.cs.wisc.edu/~bart/537/lecturenotes/titlepage.html)
* [OS: Three Easy Pieces](http://pages.cs.wisc.edu/~remzi/OSTEP/)
* [mirageOS](https://mirage.io/) - A programming framework for building type-safe, modular systems.
* [OS Dev](https://wiki.osdev.org/Main_Page) \([Tutorials](https://wiki.osdev.org/Tutorials)\)
* [Raspberry Pi OS](https://github.com/s-matyukevich/raspberry-pi-os) - Learning operating system development using Linux kernel and Raspberry Pi.
* [Create OS from scratch](https://github.com/cfenollosa/os-tutorial)
* [How to Make a Computer Operating System](https://samypesse.gitbook.io/how-to-create-an-operating-system/) \([Code](https://github.com/SamyPesse/How-to-Make-a-Computer-Operating-System)\)
* [Plan 9 from User Space](https://github.com/9fans/plan9port) - Port of many Plan 9 libraries and programs to Unix.
* [Jehanne](https://github.com/JehanneOS/jehanne) - Simple operating system.
* [Unik](https://github.com/solo-io/unik) - Unikernel & MicroVM Compilation and Deployment Platform.
* [SPDK](https://spdk.io/) - Storage Performance Development Kit Provides a set of tools and libraries for writing high performance, scalable, user-mode storage applications.
* [Writing an OS in Rust](https://os.phil-opp.com/) \([Code](https://github.com/phil-opp/blog_os)\)
* [intermezzOS kernel](https://github.com/intermezzOS/kernel) - Hobby operating system, in Rust.
* [The intermezzOS book](http://intermezzos.github.io/book/) \([Code](https://github.com/intermezzOS/book)\)
* [Write your own Operating System \(2017\)](https://www.youtube.com/playlist?list=PLHh55M_Kq4OApWScZyPl5HhgsTJS9MZ6M)
* [Operating Systems: From 0 to 1](https://tuhdo.github.io/os01/) - Bootstrap yourself to write an OS from scratch. A book for self-learner.
* [Introducing Mercury OS \(2019\)](https://medium.com/@jasonyuan/introducing-mercury-os-f4de45a04289)
* [Nanos](https://github.com/nanovms/nanos) - New kernel designed to run one and only one application in a virtualized environment.
* [BootOS](https://github.com/nanochess/bootOS) - Monolithic operating system in 512 bytes of x86 machine code. \([HN](https://news.ycombinator.com/item?id=20569438)\)
* [Ask HN: Recommended resources to learn the Linux kernel and OS theory? \(2019\)](https://news.ycombinator.com/item?id=20809666)
* [Soso](https://github.com/ozkl/soso) - Simple unix-like operating system written in Nasm assembly and mostly in C.
* [swieros](https://github.com/rswier/swieros) - Tiny and fast Unix-ish kernel \(based on xv6\), compiler, and userland for fun, education, and research.
* [A dream of an ultimate OS \(1995\)](http://okmij.org/ftp/papers/DreamOSPaper.html) \([HN](https://news.ycombinator.com/item?id=20754592)\)
* [Input/Output Subsystem in Singularity Operating System \(2011\)](http://students.mimuw.edu.pl/~md234040/master.pdf)
* [Commute talk: How to start building an OS? \(2019\)](https://www.youtube.com/watch?v=fqllFKjEZAo)
* [Making a RISC-V Operating System using Rust](https://osblog.stephenmarz.com/index.html) \([HN](https://news.ycombinator.com/item?id=21446079)\)
* [Mu: Sketching out a minimal system programming language \(2019\)](http://akkartik.name/post/mu-2019-2) \([Lobsters](https://lobste.rs/s/e39f2x/mu_sketching_out_minimal_system)\)
* [ioping](https://github.com/koct9i/ioping) - Simple disk I/0 latency measuring tool.
* [Awesome eBPF](https://github.com/zoidbergwill/awesome-ebpf) - BPF, as in Berkeley Packet Filter, is an in-kernel virtual machine running programs passed from user space.
* [What are required knowledge in order to build an OS? \(2020\)](https://www.reddit.com/r/osdev/comments/egzwa0/what_are_required_knowledge_in_order_to_build_an/)
* [Krabs](https://github.com/ellbrid/krabs) - x86 bootloader written in Rust.
* [oreboot](https://github.com/oreboot/oreboot) - Fork of coreboot, with C removed, written in Rust.
* [MIT Operating Systems Engineering course using RISC-V](https://pdos.csail.mit.edu/6.828/2019/schedule.html)
* [fectl](https://github.com/fafhrd91/fectl) - Client/server system that allows its users to monitor and control a number of processes on UNIX-like operating systems.
* [1001 Ways of Implementing a System Call \(2019\)](https://x86.lol/generic/2019/07/04/kernel-entry.html)
* [How I Switched To Plan 9 \(2019\)](http://helpful.cat-v.org/Blog/2019/12/03/0/)
* [Operating Systems course notes \(2013\)](https://www.cs.uic.edu/~jbell/CourseNotes/OperatingSystems/)
* [Computer Simulation and History](http://simh.trailing-edge.com/) \([Code](https://github.com/simh/simh)\)
* [HiddenVM](https://github.com/aforensics/HiddenVM) - Use any desktop OS without leaving a trace.
* [Programmer's critique of missing structure of operating systems \(2020\)](http://blog.rfox.eu/en/Programmer_s_critique_of_missing_structure_of_oper.html)
* [LeetCode OS Questions](https://leetcode.com/discuss/interview-question/operating-system?currentPage=1&orderBy=most_votes&query=)
* [DLS: Functional Foundations for Operating Systems course \(2018\)](https://blogs.cs.st-andrews.ac.uk/csblog/2018/01/24/dls-functional-foundations-for-operating-systems/)
* [System Programming course](http://cs241.cs.illinois.edu/coursebook/) - High-quality, open-source introductory systems programming textbook. \([Code](https://github.com/illinois-cs241/coursebook)\)
* [Green Threads Explained in Rust](https://cfsamson.gitbook.io/green-threads-explained-in-200-lines-of-rust/) \([Code](https://github.com/cfsamson/example-greenthreads)\) \([Reddit](https://www.reddit.com/r/rust/comments/bzp0cz/green_threads_explained_in_200_lines_of_rust/)\)
* [Solo5](https://github.com/Solo5/solo5) - Sandboxed execution environment for unikernels.
* [Mbox](https://pdos.csail.mit.edu/archive/mbox/) - Lightweight sandboxing mechanism that any user can use without special privileges in commodity operating systems. \([Code](https://github.com/tsgates/mbox)\)
* [Awesome Plan9](https://github.com/henesy/awesome-plan9)
* [Albatross](https://github.com/hannesm/albatross) - Orchestrate and manage MirageOS unikernels with Solo5.
* [Labs for RustOS](https://tc.gts3.org/cs3210/2020/spring/lab.html)
* [Little book about OS development](https://littleosbook.github.io/) \([Code](https://github.com/cstack/osdev)\)
* [Green Threads Explained](https://c9x.me/articles/gthreads/intro.html) \([HN](https://news.ycombinator.com/item?id=14439615)\)
* [Fibers under the magnifying glass \(2018\)](http://www.open-std.org/JTC1/SC22/WG21/docs/papers/2018/p1364r0.pdf)
* [Notes on the Plan 9 3rd Edition Kernel Source](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.75.5409&rep=rep1&type=pdf) \([Lobsters](https://lobste.rs/s/tnm3rc/notes_on_plan_9_3rd_edition_kernel_source)\)
* [Tutorial - Write a System Call \(2016\)](https://brennan.io/2016/11/14/kernel-dev-ep3/)
* [Zub VM](https://github.com/nilq/zub-vm) - Super-fast, stack-based virtual machine for dynamic languages.
* [Genode Operating System Framework Foundations](https://genode.org/documentation/genode-foundations-20-05.pdf)
* [The Benefits and Costs of Writing a POSIX Kernel in a High-Level Language \(2019\)](https://pdos.csail.mit.edu/papers/biscuit:thesis.pdf)
* [Sol — a sunny little virtual machine \(2012\)](https://rsms.me/sol-a-sunny-little-virtual-machine) \([HN](https://news.ycombinator.com/item?id=23437511)\)
* [OS Development Tutorials](http://www.osdever.net/tutorials/)
* [Modern Operating Systems 3rd edition book](http://stst.elia.pub.ro/news/SO/Modern%20Operating%20System%20-%20Tanenbaum.pdf) - 4th edition available too.
* [Learning operating system development using Linux kernel and Raspberry Pi](https://s-matyukevich.github.io/raspberry-pi-os/) \([HN](https://news.ycombinator.com/item?id=23611081)\)
* [The OS Classics \(2020\)](https://www.allthingsdistributed.com/2020/07/the-os-classics.html)
* [Operating System Design: The Xinu Approach](https://xinu.cs.purdue.edu/)
* \[Operating Systems Design & Implementation MINIX Book\]\([http://index-of.es/EBooks/Operating%20Systems%20Design%20&%20Implementation%203rd%20Edition\(1\).pdf](http://index-of.es/EBooks/Operating%20Systems%20Design%20&%20Implementation%203rd%20Edition%281%29.pdf)\)

