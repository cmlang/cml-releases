# CML Compiler 2017.10.28-alpha Release Notes

# Features:

- Functions now on the top-level of the compilation unit, along with template functions.
- Generating Java code for functions defined in CML.
- Generating Java code correctly in lambdas that access the outer scope.

# Known Issues:

- Order of properties in association may cause compilation errors of generated code.
- Missing some conditional expressions defined in language spec.
- Not supporting definition of functions in CML; only as templates.
- Not possible to define constraints for constructors (ex.: poj/pop does not support multiple inheritance)
- Not supporting annotations.
- Outer scope not accessible in parameterless lambda, including "self".
- Missing cross join code generation.
- Stack overflow in type inference with cyclical derived properties.
- Tuple type not supported as the type of properties.
- Modules need to override constructor in order to provide own function templates.
- Missing the rest() function in cml_base.
- Should attributes be allowed to use other attributes in initialization?
- Attribute initialized with none is being converted to a literal; not to path.
- What should happen if an inherited association property is redefined as derived?
- Code generation broken for secondary constructor with defaults in the cmlc targets.
