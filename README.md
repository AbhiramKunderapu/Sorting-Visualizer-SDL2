# Sorting Visualizer (SDL2, C++)

A desktop application to visualize sorting algorithms using SDL2 and C++.

## Features
- Visualizes Bubble Sort, Selection Sort, Insertion Sort, Merge Sort, and Quick Sort
- Real-time graphical animation of sorting process
- Interactive console menu for algorithm selection
- Object-oriented design for easy extension

## Build Instructions
1. **Install SDL2 development libraries** for MinGW (32-bit) from [SDL2 Downloads](https://www.libsdl.org/download-2.0.php).
2. **Extract** the SDL2 package and note the `include` and `lib` paths (e.g., `SDL2-2.28.5/i686-w64-mingw32/include` and `SDL2-2.28.5/i686-w64-mingw32/lib`).
3. **Compile** with:
   ```sh
   g++ sorting-visualiser-oops.cpp -I"SDL2-2.28.5/i686-w64-mingw32/include" -L"SDL2-2.28.5/i686-w64-mingw32/lib" -lSDL2main -lSDL2 -o sorting-visualiser.exe
   ```
4. **Copy** `SDL2.dll` from `SDL2-2.28.5/i686-w64-mingw32/bin/SDL2.dll` to your project directory (next to the `.exe`).
5. **Run** the program:
   ```sh
   ./sorting-visualiser.exe
   ```

## Usage
- Follow the console menu to select a sorting algorithm to visualize.
- Watch the SDL2 window for the animated sorting process.

## .gitignore
Add the following to a `.gitignore` file to avoid committing binaries and DLLs:
```
sorting-visualiser.exe
SDL2.dll
*.o
*.obj
*.pdb
*.exe
*.dll
```

## License
MIT (or specify your preferred license) 