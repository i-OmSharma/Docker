Application Layer
        |
        |
 Host OS Kernel
        |
        |
    hardware

Docker use the kernel of the host machine, and virtualise only the application layer.-->leds to docker lightweight and faster.

Virtual machine virtualise both the kernal and the application layer.-->vm are huge in sizes and makes them slow.

VM are compatble with all undelying OS, VM virtaulise the host kernels. VM will use there own kernel.

DockerDesktop adds a lightweight hyperviser system, which internally use a light weight linux based distro.
which helps us to run containers on nonlinux sys.