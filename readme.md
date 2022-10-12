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

## Valgrind: 
Run the following command to show valgrind output
```
valgrind --leak-check=full --track-origins=yes ./app/shell-app
```

## KCachegrind Memory Profiler Output via Command line
```
valgrind --tool=callgrind ./app/shell-app
```
-Open callgrind.out.XXX file where XXX will be the process identifier in build folder