# CML Compiler 2017.09.27-alpha Release Notes

# Features:

- When running the test task, fixed the displayed test name and the test selection by name.
- Improved generation of boolean getters in Java; generating the not operator correctly.
- Improved generation of paths in Python and Java; taking into account different combination of sequences and optionals.
- Path now finds members in ancestors, and propagates de cardinality of optional types.
- Finding properties in ancestors in property validation.
- Allowing naming convention on the CML source to differ from naming conventions in Java.
- Loading source files from cml_base module.
- New built-in functions: empty(), present(), first(), last(), exists(), all(), select(), reject(), and collect().
- New type check operators: 'is' and 'isnt'
- New type cast operators: 'as!' and 'as?'
- Marking Optional[] in the getter results in generated Python code.
- Abstract concepts now use the "abstraction" keyword; "abstract" is no longer a keyword.
- The test task now allows the verification of compilation errors in tests.
- Introduced the referential equality/inequality operators.
- Verifying the type compatibility of boolean, relational and referential operators.
- Verifying the type compatibility of unary expressions.
- Better error messages for type incompatibility of infix operators.
- Disallowing the combination of infix operands of different kinds.
- Catching invalid expressions as arguments of invocations.
- Formatted printing of syntax errors.
- Source dir may now have multiple source files and sub-dirs.
