# CML Compiler 2017.10.03b-alpha Release Notes

# Features:

- Paths containing optional types that terminate in boolean are now handled specially and return false if intermediate optional types are empty.
- Property type made required if expression inferred as optional but type is boolean.

# Known Issues:

- Special handling of boolean-terminated paths doesn't quite work yet when there are multiple intermediate optionals in the path.
