# What is Clean Code?

Readability:
Clear Naming Conventions: Use descriptive and meaningful names for variables, functions, and classes.
Consistent Formatting: Adhere to a consistent style guide for indentation, spacing, and line breaks.
Logical Structure: Organize code logically with a clear beginning, middle, and end.

Understandability:
Self-Documenting Code: Write code that explains itself through clear and concise logic.
Simplicity and Clarity: Avoid complex and convoluted logic.
Consistent Patterns: Use consistent design patterns and practices throughout the codebase.

Modifiability:
Modular Design: Structure code into small, independent modules or components.
Loose Coupling: Minimize dependencies between modules to reduce the impact of changes.
Refactoring: Regularly refactor code to improve its structure without changing its functionality.

# Why does Clean Code Matter?

- Technical debt is the accumulation of suboptimal code that can slow down development and increase the risk of bugs
- Improved collaboration in teams by making code easier to read, understand, and modify
- Fewer bugs and faster debugging due to cleaner and more maintainable code

# Key Principles

KISS: readability and maintainability
DRY: maintainability and modifiability
YAGNI: avoid unnecessary complexity -> readability and maintainability

Many more concepts like SOLID, GRASP, etc. 
SOLID: Single Responsibility Principle, Open/Closed Principle, Liskov Substitution Principle, Interface Segregation Principle, Dependency Inversion Principle
GASP: General Responsibility Assignment Software Patterns

# Readability First

Comments should explain why, not what. If you need to explain what a function does, it's not named well.

PEP8: many more rules but most of them can easily be automated with tools like Black, Flake8, etc.

Never use dunder (__) for your own variables. They are reserved for Python's internal use. They involve name mangling.

Name mangling: __var -> _ClassName__var -> _MyClass__var (name mangling)

# Functions Should Do One Thing Well

Watch for an "and" in the function name. If you can't describe what the function does without using "and", it's doing too much.

# Testable Code is Clean Code

Pytest benetfits:
- Simple Syntax: pytest has a simpler and more expressive syntax, making it easier to write and understand tests.
- Fixtures: pytest uses fixtures which are more flexible and powerful than unittest's setup and teardown methods.
- Parameterized Testing: pytest supports parameterized testing, allowing you to run a test with multiple sets of inputs more easily.