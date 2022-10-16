# Programs - CMake

## ...

- MSYS does not have "make".
- You need to tell CMake to use "mingw32-make".

References

- cmake MSYS Makefiles generator missing
  - https://stackoverflow.com/questions/37365355/cmake-msys-makefiles-generator-missing

## ...
-DCMAKE_MAKE_PROGRAM=mingw32-make

References

- CMAKE_MAKE_PROGRAM not found
  - https://stackoverflow.com/questions/6141608/cmake-make-program-not-found
