# Aggregate Types

GLSL supports the following aggregate types

* Vectors
* Matrices

### Vectors

*Vectors* can be constructed with the following basic types

* int
* uint
* float
* double
* bool

The *Vectors* supported have the following number components

* two
* three
* four

| Basic Base Type   |      2D Vector      |  3D Vector |  4D Vector |
|:----------:|:-------------:|:------:|:------:|
| int |  ivec2  | ivec3 | ivec4 |
| uint |  uvec2  | uvec3 | uvec4 |
| float |  vec2  | vec3 | vec4 |
| double |  dvec2  | dvec3 | dvec4 |
| bool |  bvec2  | bvec3 | bvec4 |

### Matrices

*Matrices* can be constructed with the following basic types

* float
* double

| Basic Base Type   |      Matrix Types |
|:----------:|:-------------|
| float |  mat2   mat3  mat4 |
| float |  mat2x2   mat2x3  mat2x4 |
| float |  mat3x2   mat3x3  mat3x4 |
| float |  mat4x2   mat4x3  mat4x4 |
| double |  dmat2   dmat3  dmat4 |
| double |  dmat2x2   dmat2x3  dmat2x4 |
| double |  dmat3x2   dmat3x3  dmat3x4 |
| double |  dmat4x2   dmat4x3  dmat4x4 |
