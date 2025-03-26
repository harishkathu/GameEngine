# GameEngine

Learnig OpenGl and GameEngine development

## How to Build (VS2017)

```bash
# Build CMake defulat VS Studio 2017 generator given you have VS2017 installed 😄
cmake -S . -B .

# To build project and generate executable (.exe)
cmake --build ./build
```

## To use Nvim (compile_commands.json)

Build CMake with MinGW as generator to generate the compile_commands.json

NOTE: .clangd is already set up to point to the correct directory 😃

```bash
cmake -G "MinGW Makefiles"-S . -B ./nvim_build
```
