# phoenix-rtos-project

Sample project using Phoenix-RTOS with helloword app. Built and tested on installation of Fedora 26 with little fixes applied on original Phoenix-RTOS version (if you wish to build on Fedora please use thewith little fixes applied on original Phoen 'fedora' branch).

### Building

1. Clone the repository and *cd* into it:
````bash
git clone https://github.com/SuperNowyNick/phoenix-rtos-helloworld/phoenix-rtos-project.git
cd phoenix-rtos-helloworld/
````
2. Initialize and update git submodules:
```bash
git submodule update --init --recursive
```

3. Build and install toolchains for all required target architectures:
````bash
   - Build the toolchain:
	(cd phoenix-rtos-build/toolchain/ && ./build-toolchain.sh i386-pc-phoenix ~/toolchains/i386-pc-phoenix)

   - Add toolchain binaries to PATH variable:
	export PATH=$PATH:~/toolchains/i386-pc-phoenix/i386-pc-phoenix/bin/
````
4. Build the project:
   - Run build.sh script:
	./build.sh

````
After the build successfully completes, kernel and disk images will be created and placed in the *_boot* directory.

### Starting the image

Run script in the main folder:
        ./run.sh
