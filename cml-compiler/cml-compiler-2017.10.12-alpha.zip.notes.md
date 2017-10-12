# CML Compiler 2017.10.12-alpha Release Notes

# Features:

- Improved performance of Java's association implementation by using LinkedHashSet.
- Implemented the following functions in cml_base: concat(seq1, seq2), count(seq), distinct(seq)

# Known Issues:

- Special handling of boolean-terminated paths doesn't quite work yet when there are multiple intermediate optionals in the path.
- Not yet generating code for the String interpolation operator ("%").
- Order of properties in association may cause compilation errors of generated code.
- Missing some conditional expressions defined in language spec.
- Not supporting definition of functions in CML; only as templates.
- Not possible to define constraints for constructors (ex.: poj/pop does not support multiple inheritance)
- Not supporting annotations.
