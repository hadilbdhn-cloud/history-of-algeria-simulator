# History of Algeria Database System

## Compile & Run

```bash
make        # compile
./algeria   # run

# Or manually:
gcc -I./include -Wall src/utils.c src/linked_list.c src/stack.c \
    src/bst.c src/recursion.c src/main.c -o algeria -lm
./algeria
```

## Project Structure
```
Algeria_DB/
├── include/       ← headers (.h)
├── src/           ← implementations (.c) — all bugs fixed
├── data/          ← sample personalities.txt
├── Makefile
└── README.md
```

## Modules
| Module | File | Features |
|--------|------|----------|
| 2 – Linked Lists & Queues | linked_list.c | insert, delete, sort, merge, palindrome, queue ops |
| 3 – Stacks               | stack.c       | push/pop, sort, convert, historical ops |
| 4 – BST                  | bst.c         | traversals, LCA, mirror, merge, balance |
| 5 – Recursion            | recursion.c   | strings, files, math, permutations, subsequences |

## Bugs Fixed
1. `windows.h` → portable ANSI escape codes (`\033[1;32m` etc.)
2. `editDistance()`: 3-arg `min()` replaced with `min3()` macro
3. Duplicate `stackToList` removed from `utils.c`
4. Duplicate `countWords` removed from `recursion.c`
5. Missing `mergeDLLs` + `convertDLLToBST` implemented in `bst.c`

to run this project successfully you must first install dependencies (raylib) because we used raylib as the gui library, here are the commands to run:

    for kali linux pcs:
  
# 1. Update your system package manager
sudo apt update

# 2. Install the core compiler tools (gcc, g++, make)
sudo apt install build-essential -y

# 3. Navigate into your project directory where the 'Makefile' is located
cd ~/Desktop/algeria/Algeria_DB

# 4. Clean up any old, stuck compilation files or Windows files
make clean

# 5. Compile the source code into a native Linux application
make# History of Algeria Database System

## Compile & Run

```bash
make        # compile
./algeria   # run

# Or manually:
gcc -I./include -Wall src/utils.c src/linked_list.c src/stack.c \
    src/bst.c src/recursion.c src/main.c -o algeria -lm
./algeria
```

## Project Structure
```
Algeria_DB/
├── include/       ← headers (.h)
├── src/           ← implementations (.c) — all bugs fixed
├── data/          ← sample personalities.txt
├── Makefile
└── README.md
```

## Modules
| Module | File | Features |
|--------|------|----------|
| 2 – Linked Lists & Queues | linked_list.c | insert, delete, sort, merge, palindrome, queue ops |
| 3 – Stacks               | stack.c       | push/pop, sort, convert, historical ops |
| 4 – BST                  | bst.c         | traversals, LCA, mirror, merge, balance |
| 5 – Recursion            | recursion.c   | strings, files, math, permutations, subsequences |

## Bugs Fixed
1. `windows.h` → portable ANSI escape codes (`\033[1;32m` etc.)
2. `editDistance()`: 3-arg `min()` replaced with `min3()` macro
3. Duplicate `stackToList` removed from `utils.c`
4. Duplicate `countWords` removed from `recursion.c`
5. Missing `mergeDLLs` + `convertDLLToBST` implemented in `bst.c`

to run this project successfully you must first install dependencies (raylib) because we used raylib as the gui library, here are the commands to run:

    for kali linux pcs:
  
# 1. Update your system package manager
sudo apt update

# 2. Install the core compiler tools (gcc, g++, make)
sudo apt install build-essential -y

# 3. Navigate into your project directory where the 'Makefile' is located
cd ~/Desktop/algeria/Algeria_DB

# 4. Clean up any old, stuck compilation files or Windows files
make clean

# 5. Compile the source code into a native Linux application
make
# 6. Check the directory to see the newly generated Linux executable file
ls -l

# 7. Run your native Linux app (Replace 'algeria' with the green-colored binary file name if it differs)
./algeria

    for windows pcs:

Step 1: Install the Compiler
Download and install w64devkit or MinGW-w64.

Make sure gcc and make (or mingw32-make) are added to your Windows Environment Path variables.

Step 2: Open Command Prompt (cmd) or PowerShell and run:
PowerShell
# 1. Navigate to the project folder (Update the path depending on where you saved it)
cd C:\Users\YourUsername\Desktop\algeria\Algeria_DB

# 2. Clean previous build artifacts
mingw32-make clean

# 3. Compile the source code natively for Windows 
mingw32-make

# 4. Run the newly created Windows executable application
.\algeria.exe
