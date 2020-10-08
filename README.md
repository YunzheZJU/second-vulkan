# second-vulkan

Learning vulkan.

System Requirements:
* **Windows 10 64bit**
* **CMake 3.17**
* **Vulkan SDK** This ensures glslc.exe exists to compile shaders by running `shaders/compile.bat` before building executables
* C Compiler: **MSVC(Microsoft Visual Studio 2019)** with x64(amd64) as the target architecture
* `vulkan-1.dll` should be found under `Windows/system32`, or you must provide one besides the built executable
* A vulkan compatible physical device, this usually means a modern graphic card, or an embed one in an Intel CPU.

All necessary developing libraries are included in `/includes` and `/lib`:
* `include/GLFW` is copied from `glfw-3.3.2.bin.WIN64/include`
* `include/vulkan` is copied from `VulkanSDK/1.2.148.1/Include`
* `include/glm` is copied from `glm`@0.9.9.8.
* `include/stb_image.h` is copied from [stb/images](https://raw.githubusercontent.com/nothings/stb/master/stb_image.h).
* `lib/glfw3.lib` is copied from `glfw-3.3.2.bin.WIN64/lib-vc2019`
* `lib/vulkan1.lib` is copied from `VulkanSDK/1.2.148.1/Lib`
