# *uniform*

The *uniform* type modifier has the following features

* **Global Declaration**: Any *uniform* variable MUST be declared as a global variable so that it can be shared across all the shader stages (vertex & fragment shaders) enabled in a program.
* **Assigning a value**: A *uniform* variable is assigned a value ONLY by its application before the execution of any of its shaders. 
* **Read-only in shaders**: A *uniform* variable's value cannot be assigned/modified by a shader.

### Accessing & Modifying *uniform* variables

**Accessing in the application**

Use the *glGetUniformLocation()* routine

**Modifying in the application**

Use the *glUniform_()* or the *glUniformMatrix_()* routines.
