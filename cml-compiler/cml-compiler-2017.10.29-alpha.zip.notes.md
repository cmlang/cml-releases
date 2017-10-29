# CML Compiler 2017.10.29-alpha Release Notes

# Features:

- Inferring result type of functions defined by expressions; thus, allowing functions defined by expressions to omit the result type.
- Fixed Java code generation of functions defined in CML; converting cardinality correctly.
- Converting sequence to seq() in many of the cml_base functions; supports cases where the variable has not yet been converted.
- Using target language's naming convention on function invocation.
- Java targets now converting concat's single-cardinality args to sequence.
- Implemented functions includes/excludes in the cml_base module.
- Accepting a lambda as the argument of a parameter with a non-function type if the lambda has no parameters. It is evaluated prior to invocation in the scope of invocation; not on the scope of the function. This allows includes/excludes functions to be used in comprehensions.

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
