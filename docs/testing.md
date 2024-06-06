# Testing Guide

We need to ensure that each component has test coverage of more than 80 percent.

## Testing Frameworks

- **Unit Testing:** Jest - React testing library
- **End-to-End Testing:** Cypress

## Test Structure

```txt
src/
├── tests/
│ ├── components/
│ ├── containers/
│ └── ...
├── App.test.tsx
└── ...
```

## Running Tests

To run unit tests:

```bash
yarn test
yarn test:coverage
```

To run end-to-end tests:

```bash
npx cypress open
```

### Writing Tests

Use describe and it blocks for structuring tests.
Mock API calls using jest.mock or cy.intercept.

---

[Go back to Readme](../README.md)
