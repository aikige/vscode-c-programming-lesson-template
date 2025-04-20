# Visual Studio Code Template to Learn C Programming with LLVM

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

This setting assumes LLVM based C programming environment (i.e. uses `clang` as compiler and `lldb` as debugger) and this section provides environment which is verified to work.

## Windows

[scoop]:https://scoop.sh/
[LLVM]:https://www.llvm.org/
If you do not have `clang` and `lldb` installed, it is recommended to install [LLVM] environment (which includes `clang` and `lldb`) using [scoop].

```
scoop install main/llvm
```

## MacOS

Please follow instruction in VS Code official site:
* [Using Clang in Visual Studio Code](https://code.visualstudio.com/docs/cpp/config-clang-mac)
