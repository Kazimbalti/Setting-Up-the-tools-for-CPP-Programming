# Setting-Up-the-tools-for-CPP-Programming
This is the setting Up tools for C++ programming on window, Linux and MacOS. 
1. Tools
2. Installing C++ Compilers on Windows
3. Installing VS Code on Windows
4. Configuring Visual Studio Code for C++ on Windows
5. Installing C++ Compilers on Linux
6. Installing Visual Studio Code on Linux
7. Configuring Visual Studio Code for C++ on Linux
8. Installing C++ Compilers on MacOs
9. Installing Visual Studio Code on MacOs
10. Configuring Visual Studio Code for C++ on MacOs
11. Online Compilers
## 1. Tools
### IDEs:
#### IDEs for Window
1. Visual Studio Code
2. Microsoft Visual Studio
3. CodeLite
#### IDEs for Ubuntu
1. Visual Studio Code
2. QT Creator
3. CodeLite
#### IDEs for MacOS
1. Visual Studio Code
2. XCode
3. CodeLite
### Compilters
Compilters is a tool that transform your C++ code into a format that can run directly on a hardware.
#### Compiler for Window
1. MingW 
2. Msvc
3. Clang llvm
#### Compiler for Ubuntu
1. GCC
2. Clang llvm
#### Compiler for MACOS
1. GCC
2. Clang llvm
3. Clang Apple
## 2. Installing C++ Compilers on Windows
First of all you have to visit [C++ compiler support](https://en.cppreference.com/w/cpp/compiler_support) to check your compiler supports.
To download the GCC and Clang llvm on your machine go to this website [WinLibs](https://winlibs.com/) and download the latest release version i.e., ![clang](https://user-images.githubusercontent.com/32608321/159446993-f3f78aa7-e449-40fc-b8dd-296b55afe411.PNG)
Then go to the downloaded folder and extract it and place it somewhere on your system, where you find mingw64 folder.
Go to the mingw64/bin folder and copy it i.e., your_directory/ming64/bin and type env from the start menu "Edit the system environment variable" will popup and edit the environment variable according to below image:
![github](https://user-images.githubusercontent.com/32608321/159451849-4398ae0d-0b5c-46d2-954e-85a13164240c.PNG)
Now to test the environment_variables/compiler is working open the command prompt and type "g++ --version" as shown in figure below:

![image](https://user-images.githubusercontent.com/32608321/159466927-5f60bf09-d6ec-4ae8-b62f-17fae5ea0ae5.png)

Now the C++ compiler is ready for MingW project.

## 3. Installing VS Code on Windows
Download visual studio code from this link [Visual Studio Code](https://code.visualstudio.com/) and install it accordingly.
Open the Visual Studio code and first install the package from the extensions. So first install the C/C++ Intellisence, debuggin, and code browsing package as shown in figure.

![image](https://user-images.githubusercontent.com/32608321/159468907-f37cb53b-27e9-4226-bc88-aa52e3aae8dc.png)

## 4. Configuring Visual Studio Code for C++ on Windows
Here we will show how to connect the IDEs (Visual Studio Code) to the compiler Mingw (g++).
Open up the Visual Studio code and make a folder i.e., First_Program and make a new file inside this First_Program folder.
>>First_Program
    >> main.cpp
write a simple program inside the main.cpp file and click on the terminal bar, from where you open/click on the configuration tasks, as shown in figure

![image](https://user-images.githubusercontent.com/32608321/159682546-ae320ae4-7cfc-4ff3-ad0b-8983bf0f4638.png)

In configuration task menu go to the g++.exe and open it, as shown in figure

![image](https://user-images.githubusercontent.com/32608321/159683686-c844559e-be66-4098-8451-ea0de8695b6f.png)

it will show a tasks.json file inside the .vscode file. as shown below
![image](https://user-images.githubusercontent.com/32608321/159683832-000d81a0-0c44-44f0-854b-4cb3a9a5870b.png)

Modify the tasks.json file for C++ 20 version by adding "-std=c++20" in args after -g on line 10, as shown in figure

![image](https://user-images.githubusercontent.com/32608321/159685374-fd9594d5-cd03-4e16-887b-5d044464a463.png)

Finally go to the Terminal/new_terminal and then go to Terminal/Run_Task, it will bind you program to build with GCC 11.2.0, as shown below

![image](https://user-images.githubusercontent.com/32608321/159686301-86d0a678-12a3-4310-8323-9ac17c4c1a68.png)

Finally you have build your program.
you can run ./main.exe binary directly from the terminal.

Thats all for configuring visual studio code with the compiler in windows.


