# Compiling Shaders

The GLSL shaders in a program can be compiled and linked using the OpenGL API.

### Similarities with Compiling a C program

A regular C program is compiled in the following way:

* **Compiling Phase**: A program is fed to a **compiler** to be analyzed and checked for errors; The compiler generates an *object code* of the given program.
* **Linking Phase**: The *object code* generated in the previous step and a set of other previously generated *object code* files are fed to a **linker**, which *links* all the *object code* files to generate an *executable program*.

A GLSL program is compiled in a similar way, but by using the OpenGL API.

### Shader Compiling Phase

A shader program that has to be used in an application should be compiled in the following way

* **Create a Shader Object**: Create a shader object to compile the shader source into
* **Associate Shader Source with Shader Object**: Associate the source code of the shader with the shader object created in the previous step
* **Compile Shader Source**: Compile the shader source associated with the shader object

After the compilation, verify that the shader was compiled successfully.

### Shader Linking Phase

* **Create a Shader Program**: Create a shader program that can be attached with shader objects
* **Attach Shader Objects**: Attach the shader objects to the shader program in the previous step
* **Link Shader Program**: Link the shader program to create the shader

After the linking process, verify that the shader program was linked successfully. 
The generated shader can be used for processing vertices or fragments depending on what kind of shader it is.

### OpenGL API for Shader Compilation and Linking

**Creating a Shader Object**

A shader object can be created by calling the *glCreateShader()* function. The prototype of the function is

```GLSL
GLuint glCreateShader(GLenum type)
```

The *type* can take any one of the following values

* GL_VERTEX_SHADER
* GL_FRAGMENT_SHADER
* GL_TESS_CONTROL_SHADER
* GL_TESS_EVALUATION_SHADER
* GL_GEOMETRY_SHADER

The return value is 

* 0 in case of an error (or)
* > 0 
