# Introduction to Test and Behavior Driven Development

## Module 1: Introduction to Testing
https://www.coursera.org/learn/test-and-behavior-driven-development-tdd-bdd/home/module/1

### Video Notes: The Importance of testing

- Design principles for Apollo
    - Use a high-level language
    - Divide into jobs
    - Restart on failure
    - Checkpoint good state
    - Hardware monitors the software
    - Send telemetry
- You don't just fix software, you write test cases that reproduces the error and then fix the software.
- You can only test what you know.
- Interactions with complex systems are hard to predict. Reproducing errors in test cases leads to more robust software.

### Video Notes: Why Developers Don't Test

Testing gives confidence in deployment, remind future maintainers (and future you) of what's working and what's not working.

### Video Notes: Testing Levels and Release Cycle

Levels:
- Unit: testing each module in isolation, both good and bad cases. TDD happens here.
- Integration: module interaction testing. BDD happens here.
- System: entire process testing, whole system, staging, close to production.
- Acceptance: User acceptance testing, like production.

Environments:
- Development (unit testing, build, packaging)
- Test: (component, integration, performance)
- Stage: (performance, user acceptance)
- Production: (performance, system)

### Video Notes: TDD and BDD

BDD:
- focusus on the behavior of the system from the outside
- works great for integration testing
- common syntax between dev and stakeholders
- ensures you're building the right thing

TDD:
- focuses on the system from the inside
- tests drive the design
- write tests first, then write code to make the tests pass
- ensures you're building the thing right

## Module 2: Basics of Test Driven Development

### Video notes:

TDD means your unit test cases drive the design.
You write the tests first for the code you wish you had, then you write the code to make the tests pass.
TDD keeps devs focused on the code.

Workflow: Red -> Green -> Refactor -> goto Red

TDD ensures that the code is working as expected.

Automate all testing to build CI/CD pipelines.

Popular testing frameworks:
- xUnit series
- Jasmine
- Mocha
- SimpleTest

Python:
- PyUnit
- Pytest
- Doctest
- RSpec
- Nose
- Coverage

## Module 2: Methods for Test Driven Development

### Hands-on Lab: Running Tests with Nose

Nosetest setup.cfg:

```
[nosetests]
verbosity=2
with-spec=1
spec-color=1
with-coverage=1
cover-erase=1
cover-package=triangle

[coverage:report]
show_missing = True
```


