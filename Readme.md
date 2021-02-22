Unrolling Loops Sample
The Loop Unroll demonstrates a simple example of unrolling loops to improve the throughput of a DPC++ program for GPU offload.

For comprehensive instructions see the DPC++ Programming and search based on relevant terms noted in the comments.

Optimized for	Description
OS	Linux* Ubuntu* 18.04,
Hardware	Skylake with GEN9 or newer,
Software	Intel® oneAPI DPC++ Compiler
What you will learn	how to perform reduction with oneAPI on cpu and gpu
Time to complete	30 min
Purpose
The loop unrolling mechanism is used to increase program parallelism by duplicating the compute logic within a loop. The number of times the loop logic is duplicated is called the unroll factor. Depending on whether the unroll factor is equal to the number of loop iterations or not, loop unroll methods can be categorized as full-loop unrolling and partial-loop unrolling. A full unroll is a special case where the unroll factor is equal to the number of loop iterations.

Key Concepts
Basics of loop unrolling.
How to unroll loops in your program.
Determining the optimal unroll factor for your program.
License
Code samples are licensed under the MIT license. See License.txt for details.

Third party program Licenses can be found here: third-party-programs.txt

Building the loop_unroll Tutorial
Note: if you have not already done so, set up your CLI environment by sourcing the setvars script located in the root of your oneAPI installation.

Linux Sudo: . /opt/intel/oneapi/setvars.sh
Linux User: . ~/intel/oneapi/setvars.sh
Windows: C:\Program Files(x86)\Intel\oneAPI\setvars.bat

Include Files
The included header dpc_common.hpp is located at %ONEAPI_ROOT%\dev-utilities\latest\include on your development system.

Running Samples in DevCloud
If running a sample in the Intel DevCloud, remember that you must specify the compute node (fpga_compile or fpga_runtime) and whether to run in batch or interactive mode. For more information see the Intel® oneAPI Base Toolkit Get Started Guide (https://devcloud.intel.com/oneapi/get-started/base-toolkit/).

Building the loop-unroll Program for CPU and GPU
Running Samples In DevCloud
If running a sample in the Intel DevCloud, remember that you must specify the compute node (CPU, GPU, FPGA) and whether to run in batch or interactive mode. For more information, see the Intel® oneAPI Base Toolkit Get Started Guide (https://devcloud.intel.com/oneapi/get-started/base-toolkit/)

On a Linux* System
Build the program using the following cmake commands.
$ cd loop-unroll
$ mkdir build
$ cd build
$ cmake ..
$ make
Run the program
$ make run  
Clean the program
$ make clean
On a Windows* System Using Visual Studio* Version 2017 or Newer
Build the program using VS2017 or VS2019

Right-click on the solution file and open using either VS2017 or VS2019 IDE.
Right-click on the project in Solution Explorer and select Rebuild.
From the top menu, select Debug -> Start without Debugging.
Build the program using MSBuild

Open "x64 Native Tools Command Prompt for VS2017" or "x64 Native Tools Command Prompt for VS2019"
Run the following command: MSBuild loop-unroll.sln.sln /t:Rebuild /p:Configuration="Release"

## Running the sample on devcloud
clone the repo
run the ipython notebook
## The experience
## Good
It was good learning experience to work with DPC++,Had got good exposure to GPU ,FPga
## bad
Devcloud is slow at times
The learning process of DPC++ is tough

