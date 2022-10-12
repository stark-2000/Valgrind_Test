# Valgrind Exercise
---

## Basic Setup: 
Run the following commands in order
```
git clone git@github.com:stark-2000/Valgrind_Test.git
cd Valgrind_Test
mkdir build
cd build
cmake ..
make
cd app
```

## Running "Valgrind": 
Run the following command to show valgrind output
```
valgrind --leak-check=full --track-origins=yes ./shell-app
```

## Running "Function & Memory Profiler - KCachegrind": 
Install "KCachegrind" from "Ubuntu Software" app
Run the below command & open "callgrind.out.XXXXX" file located in ./build/app directory using "KCachegrind" app
```
valgrind --tool=callgrind ./shell-app
```
