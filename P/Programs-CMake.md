# Programs - CMake

## ...

- MSYS does not have "make".
- You need to tell CMake to use "mingw32-make".

References

- MinGW sh.exe must NOT be in your path
  - https://stackoverflow.com/questions/41333215/mingw-sh-exe-must-not-be-in-your-path
- CMake Error: CMake was unable to find a build program corresponding to "MSYS Makefiles". #578
  - https://github.com/tpaviot/oce/issues/578
- CMake Error: CMake was unable to find a build program corresponding to "MinGW Makefiles"
  - https://stackoverflow.com/questions/45150172/cmake-error-cmake-was-unable-to-find-a-build-program-corresponding-to-mingw-ma
- What is wrong with cmake under mingw
  - https://stackoverflow.com/questions/55093703/what-is-wrong-with-cmake-under-mingw 
- cmake MSYS Makefiles generator missing
  - https://stackoverflow.com/questions/37365355/cmake-msys-makefiles-generator-missing

## ...
-DCMAKE_MAKE_PROGRAM=mingw32-make

References

- CMAKE_MAKE_PROGRAM not found
  - https://stackoverflow.com/questions/6141608/cmake-make-program-not-found
