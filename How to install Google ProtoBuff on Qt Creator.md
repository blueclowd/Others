# Installation Guide

This is a brief guide about how to install **Google Protocol Buffer 3** on **Qt Creator**. 

To successfully set up a new enviroment for development is never an easy work.
Enthusiastically expect that this short paragraph will do any help to those struggling with the installation process. Please let me know if you have any opinions and any feedback is really appreciated.

The installation guide is tested by:
  - [Ubuntu 16.04 LTS]
  - [Google Protocol Buffer 3.0.0]
  - [Qt Creator 4.1.0]
  - Language: C++
  - Compiler: GCC x86 64bit

[Ubuntu 16.04 LTS]: <https://wiki.ubuntu.com/XenialXerus/ReleaseNotes?_ga=1.166009847.871706029.1475201071>
[Qt Creator 4.1.0]: <https://www.qt.io/ide/>
[Google Protocol Buffer 3.0.0]: <https://developers.google.com/protocol-buffers/>


### Steps

##### Step 1: Download two assential packages from the website of Google Protocol Buffer release page:
 - [protobuf-cpp-3.0.0.zip]
 - [protoc-3.0.0-linux-x86_64.zip]
 
[protobuf-cpp-3.0.0.zip]: <https://github.com/google/protobuf/releases/tag/v3.0.0>
[protoc-3.0.0-linux-x86_64.zip]: <https://github.com/google/protobuf/releases/tag/v3.0.0>
***
##### Step 2: Unzip the two packages mentioned above
***
##### Step 3: Go to the folder /protobuf-cpp-3.0.0 and type the following command one after another:

```sh
$ ./configure   
$ make 
$ make install
```
***
##### Step 4: Check if corresponding files was generated in folder /usr/local/lib (It's a default path if we didn't change it by ./configure {desired path}). Note that this is the last step of installing the Google Protocol Buffer compiler.
***
##### Step 5: After finish compiler installation. We can start to set up the project in Qt creator. We first create a C++ project in "Welcome" page and select "New Project". We simply select "Plain C++ application" to make the steps more simple. 
***
##### Step 6: Now we have an new C++ project in Qt creator. We already know that the project settings including project type and file reference are descriped in {projectName}.pro. We add a new line to make a link to the generated files in /usr/local/lib

```sh
$ LIBS += -L/usr/local/lib
```

***
##### Step 7: We have finished all the enviroment settings till now. You can check it by building the project and run it to see if the result is shown as expected. Enjoy your journey from here.


> Should you have any questions about this paragraph, please email me via:
> lhungting@gmail.com


