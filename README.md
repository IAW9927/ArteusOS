# ArteusOS
Arteus OS source code/releases

Please help me build this. Packages are in .tar.gz format.

Note: BusyBox is used as the main utilities =)

# How to build a package for ArteusOS
You need to build the source code, it ***MUST*** be static! Otherwise, the code wil fail!

Also, you MUST install it's results into a directory called "pkg".

You must be in the build directory to do this.

Commands to run:

root@dev:~# tar cvf - ./pkg/* > <package_name>

Then, you upload the file. The repo will be there at https://iaw9927.github.io/ArteusRepo/

After you have uploaded the file, please create a issue about "Add <package name> to repository".
  
Then, the package will be added and the system built.
  
Also, please grab your running kernel and /lib/modules/$(uname -r) directory zipped. Upload it and I'll add the updated kernel and modules. 
  
I am building this system for regular computers, but PLEASE use the source code and compile https://github.com/freedesktop/xorg-xserver if you want Xorg. If you for some reason nedd any component from Xf86 which you want/need, go to  https://github.com/freedesktop/ to find all source code binarys.
  
Every package MUST be compiled from source code, statically and full-features, and please ***NO*** development symbols.
  
It will make the package bigger and this is not good, because we are a team together to make this distro from scratch!
  
Can you compile Busybox with every utility and package. Use build statically and make GCC use static library. This must be done when updating the distro. You must build it and copy /lib64/ld-linux-x86-64.so.2 to your archive and upload it. This is required for starting the distro.
