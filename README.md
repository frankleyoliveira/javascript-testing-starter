# Mastering JavaScript Unit Testing

This repository contains the code and my personal notes from the video [JavaScript Unit Testing Tutorial for Beginners](https://www.youtube.com/watch?v=zuKbR4Q428o) by Mosh Hamedani. The tutorial covers the principles of unit testing, lays the foundation for Test-Driven Development (TDD), and introduces the Vitest testing framework.

### Benefits of Writing Tests

- Detect bugs early – bugs found after deployment can cost 30× to 100× more
- Refactor with confidence
- Improve overall code quality
- Serve as living documentation

### Types of Tests

- **Unit tests** – test components in isolation  
- **Integration tests** – test how components work together  
- **End-to-end (E2E) tests** – test the entire application flow  

### TDD – Test-Driven Development

1. Write a **failing test** first  
2. Write just enough code to make the test **pass**  
3. **Refactor** the code to improve structure without changing behavior  

### Popular Testing Frameworks

- **Jest**, **Mocha**, **Jasmine**, **Vitest**, **Cypress**, **Playwright**  
  > Most of these tools share similar concepts. Once you learn one, switching to another is relatively easy.

### AAA Principle

Use the **Arrange-Act-Assert** pattern when writing tests.  
Example: Testing whether a TV can be turned off:

- **Arrange** – Set up the environment and initial state (e.g., Turn on the TV)  
- **Act** – Perform the action under test (e.g., Press the power button)  
- **Assert** – Verify the expected outcome (e.g., Confirm the TV is off)  

### Getting Started with Vitest

- Install Vitest and add a "test" script in `package.json`
  - Command to run the tests: `npm t`

- Create a `tests` folder
  - Test files must end with `.test.js`

- Common Vitest functions to import in test files:
  - `describe`: used to group related tests
  - `test`: creates an individual test case
  - `it`: alias for `test`
  - `expect`: used to write assertions

### Best Practices

- Always ensure your tests are **in sync** with the production code  
- A good habit: **intentionally break a test** (e.g., change a function temporarily) to confirm your test fails properly

