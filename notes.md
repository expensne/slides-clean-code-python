# What is Clean Code?

Readability:
Conventions
Consistent Formatting
Logical Structure

Understandability:
Self-Documenting Code
Simplicity and Clarity
Consistent Patterns

Modifiability:
Modular Design
Loose Coupling
Refactoring

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

PEP8: tool support: Black, Flake8 

Never use dunder (__) for your own variables. They are reserved for Python's internal use. They involve name mangling.

Name mangling: __var -> _ClassName__var -> _MyClass__var (name mangling)

# Functions Should Do One Thing Well

Watch for an "and" in the function name. If you can't describe what the function does without using "and", it's doing too much.

# Testable Code is Clean Code

Pytest benetfits:
- Simple Syntax: pytest has a simpler and more expressive syntax, making it easier to write and understand tests.
- Fixtures: pytest uses fixtures which are more flexible and powerful than unittest's setup and teardown methods.
- Parameterized Testing: pytest supports parameterized testing, allowing you to run a test with multiple sets of inputs more easily.