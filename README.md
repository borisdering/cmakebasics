# Basic CMake C++ Setup
This repository contains a program which consumes a library. For personal use. 

## How build this simple setup
Navigate to library first 
```
// from the root folder
$ cd library
$ cmake -H. -Bbuild 
$ cd build
$ make 
```

To build the consumer program 
```
// from the root folder
$ cd consumer
$ cmake -H. -Bbuild 
$ cd build
$ make 
```

## How to exectute this program
You can run this program by 
```
// from the root folder
$ cd consumer/build/bin
$ ./consumer
```
