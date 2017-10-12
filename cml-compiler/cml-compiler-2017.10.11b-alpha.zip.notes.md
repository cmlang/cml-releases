# CML Compiler 2017.10.11b-alpha Release Notes

# Features:

- Allowing forced-casting from optional to required cardinality.
- Returning undefined type if unable to infer type of member in path.
- Inferring correctly the type of concept invocation expression.
- Supporting "+" as the String operator for concatenation.

# Known Issues:

- Special handling of boolean-terminated paths doesn't quite work yet when there are multiple intermediate optionals in the path.
- Not yet generating code for the String interpolation operator ("%").
