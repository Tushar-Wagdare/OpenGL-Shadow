# OpenGL-Shadow

## Description

This repository demonstrates the implementation of Shadow Mapping techniques in OpenGL using C++ and GLSL. It includes two separate shadow mapping approaches: Basic Shadow Mapping and Cascaded Shadow Mapping, enhancing realism by simulating shadows in the scene.

## Screenshots

##### Simple Shadow Mapping
![Basic Shadow Mapping](01_ShadowMapping/S1.png)

![Basic Shadow Mapping](01_ShadowMapping/S1.png)


##### Cascaded Shadow Mapping
![Basic Shadow Mapping](02_CascadedShadowMapping/S1.png)

![Basic Shadow Mapping](02_CascadedShadowMapping/S1.png)

## Folder Structure

*   `01_ShadowMapping`: Contains the code for the basic shadow mapping implementation.
    *   `ShadowMapping/x64/Debug`: Contains build files and output executables.
    *   `resources`: Contains model and texture assets used for testing shadows.
    *   `shaders`: Contains GLSL shader programs for rendering and shadow calculation.
    *   `x64/Debug`: Contains debug build output.
*   `02_CascadedShadowMapping`: Contains the code for the cascaded shadow mapping implementation.
    *   `CascadedShadowMapping/x64/Debug`: Contains build files and output executables.
    *   `resources`: Contains model and texture assets used for testing shadows.
    *   `shaders`: Contains GLSL shader programs for rendering and cascaded shadow calculation.
    *   `x64/Debug`: Contains debug build output.
*   `.gitignore`: Specifies intentionally untracked files.

## Dependencies

Before building and running this project, you need to install the following dependencies:

*   **GLEW (OpenGL Extension Wrangler Library):** Download GLEW and add the `include` directory and library files (e.g., `glew32.lib`) to your system environment variables.
*   **GLM (OpenGL Mathematics):** Download GLM. GLM is a header-only library, so simply copy the `glm` directory into your project's include path.

**Note:** Adding GLEW, Assimp and GLM to your system environment variables ensures that Visual Studio can find them during the build process. This typically involves adding paths to the `INCLUDE` and `LIB` environment variables.

## Build Instructions (Visual Studio 2022)

Follow these steps to build the project using Visual Studio 2022:

1.  **Clone the Repository:** Clone this repository to your local machine using the following command:
    ```bash
    git clone https://github.com/Tushar-Wagdare/OpenGL-Shadow.git
    ```
2.  **Open the Solution:** Open the `OGL.sln` file in Visual Studio 2022 within either the `01_ShadowMapping` or `02_CascadedShadowMapping` folder.
3.  **Build the Solution:** Go to `Build` -> `Build Solution` (or press `Ctrl+Shift+B`).
4.  **Ensure all dependencies are present:** Make sure all the dependencies are installed and placed in the system environment.
5.  **Run the Solution:** After building, run the executable located in the respective `x64/Debug` directory.

## Usage

After successfully building the project, you can run the executable located in the `x64/Debug` directory within either the `01_ShadowMapping` or `02_CascadedShadowMapping` folder. Explore the effect of shadows in the scene using Basic and Cascaded shadow mapping.
