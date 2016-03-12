# Two Steps of installing C/C++ Eclipse in Ubuntu 14.04

There are many tutorials teaching how to use Eclipse in Ubuntu for C/C++ writing. Most of them contains complex steps from installing the JRE, setting the JAVA path, downloading the Eclipse to installing the CDT plugins. I would like to share my two-step tutorial to achieve that.
+ Step 1: Install JRE
    - Though we attempt to write C/C++ instead of Java in Eclipse, we need to install JRE first since it is essential for running Eclipse.
    - Type '**sudo apt-get install default-jre**' in terminal
+ Step 2: Download and run eclipse
  - Download link: http://www.eclipse.org/downloads/packages/eclipse-ide-cc-developers/mars2
  - The downlaod package contains CDT (C/C++ Development Tools) so we don't need to install it afterwards. 
+ Step 3: Run Eclipse by double-clicking the icon and run the built-in helloWorld project to check if it works.

That's it. Enjoy writing C/C++ in Eclipse.