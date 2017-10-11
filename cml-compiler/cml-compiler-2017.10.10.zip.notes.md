# CML Compiler 2017.10.10 Release Notes

# Features:

- Displaying type of path as argument of invocation error.
- Allowing invocation of concepts.
- Generating code for the invocation of concepts that create instances.
- Fixed Java code generation for equality operator of optional types.

# Known Issues:

- Special handling of boolean-terminated paths doesn't quite work yet when there are multiple intermediate optionals in the path.
