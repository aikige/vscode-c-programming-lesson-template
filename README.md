# Visual Studio Code Template to Learn C Programming

This template provides `.vscode/tasks.json` and `.vscode/launch.json` files which are useful to start learning C programming using Visual Studio Code (VS Code).

## Usage

This project helps user to run an active C source code.
Here, the source code is assumed to include `main()` and not depend on external libraries or objects.

1. Prepare compiler and debugger (described later).
1. Download or clone this project.
1. Open downloaded project folder by VS Code.
1. Edit `example.c` or create new C program in the project folder.
1. Compile and run/debug active C source code by either of following method:
    1. Open command pallet and execute `Task: Run Test Task`.
    1. Click `Run and Debug` editor action button in the editor pane.
    1. Click `Run and Debug` button in activity bar.
    1. Click `Select and Start Debug Configuration button in status bar.

## Preparing C Programming Environment
[scoop]:https://scoop.sh/
[MinGW]:https://www.mingw-w64.org/
[LLVM]:https://www.llvm.org/

This setting assumes [LLVM] based C programming environment (i.e. uses `clang` as compiler and `lldb` as debugger) on MacOS environment.
And [MinGW] environment (i.e. uses `gcc` as compiler and `gdb` for debugger) on Windows.

## Windows: Preparation of MinGW Environment.

If you do not have `gcc` and `gdb` installed, it is recommended to install [MinGW] environment (which includes `gcc` and `gdb`) using [scoop].

```
scoop install main/mingw
```

### Note

* LLVM/clang/lldb is not used since scoop version of `lldb` has problem.

## MacOS: Preparation of LLVM Environment

Please follow instruction in VS Code official site:

* [Using Clang in Visual Studio Code](https://code.visualstudio.com/docs/cpp/config-clang-mac)
