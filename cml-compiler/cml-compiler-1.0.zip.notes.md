# CML Compiler 1.0 Release Notes

Release Date: 13 May 2017

# Features:

Supports CML Language 1.0 Draft:

- Concepts
    - Single / Multiple Inheritance
    - Properties
        - Attributes
        - Unidirectional Associations
        - Initialized
        - Derived
- Bidirectional Associations
- Tasks
- Expressions
- Templates:
    - Languages
        - Java
        - Python
    - Constructors
        - poj (Plain-Old-Java)
        - pop (Plain-Old-Python)
        - to be used by CML compiler's metamodel:
          (Implements multiple inheritance with interfaces and delegation.)
            - cmlc_java (for Java)
            - cmlc_python (for Python)
- Modules:
    - Importing other modules.
    - May reference concepts from another module.
    - A task can use a concept from another module.

# Known Issues

- IndexOutOfBoundsException if the task name isn't provided as the first argument to the "cml" command.
- Not yet generating code for bidirectional associations.
- Not yet verifying the invariants of the metamodel and reporting them as compilation errors.
- No type checking.
