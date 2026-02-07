## Windows

1) Open the solution in Visual Studio 2022
2) Compile as `Release`/`x64`
3) Set the startup project to the `UI` project and run

## Linux

To build under Linux you need a version of Clang or GCC that supports C++17.  

Additionally, SDL2 and the [.NET 8 SDK](https://learn.microsoft.com/en-us/dotnet/core/install/linux) must also be installed.

Once SDL2 and the .NET 8 SDK are installed, run `make` to compile with Clang.  
To compile with GCC instead, use `USE_GCC=true make`.  
**Note:** Mesen usually runs faster when built with Clang instead of GCC.

To create an AppImage, you must execute appimage.sh from the root folder, i.e., from the terminal:  Linux/appimage/appimage.sh

Alternatively, navigate to ./Linux/appimage/ and execute appimage_reldir.sh, i.e., from the terminal:  ./appimage_reldir.sh

## macOS

To build macOS, install SDL2 (i.e via Homebrew) and the [.NET 8 SDK](https://dotnet.microsoft.com/en-us/download/dotnet/8.0).  

Once SDL2 and the .NET 8 SDK are installed, run `make`.
