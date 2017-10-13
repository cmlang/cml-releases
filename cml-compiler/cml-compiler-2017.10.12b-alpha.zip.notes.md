# CML Compiler 2017.10.12b-alpha Release Notes

# Features:

- Implemented the none() function in cml_base.
- Fixed lambda scope when parameters are defined.

# Known Issues:

- Special handling of boolean-terminated paths doesn't quite work yet when there are multiple intermediate optionals in the path.
- Not yet generating code for the String interpolation operator ("%").
- Order of properties in association may cause compilation errors of generated code.
- Missing some conditional expressions defined in language spec.
- Not supporting definition of functions in CML; only as templates.
- Not possible to define constraints for constructors (ex.: poj/pop does not support multiple inheritance)
- Not supporting annotations.
- Outer scope not accessible in parameterless lambda, including "self".
- Missing cross join code generation.
- Stack overflow in type inference with cyclical derived properties.
