# javascript-unit-testing

JavaScript Unit Testing - The Practical Guide by Maximilian Schwarzmüller

## Folder Structure

# Details

<details open> 
  <summary>Click to Contract/Expend</summary>

## Section 1: Getting Started

### 4. Unit vs Integration vs E2E Tests

1. Unit Testing
2. Integration Testing
   - test the combination of building blocks (units)
   - even if all units work standalone, the combination could fail
3. End-toEnd (E2E) Testing
   - real users use your app and its features, not individual units

## Section 2: Setup & Testing Software

### 10. Which Tools Are Needed For Testing?

- Test Runner: Jest, Karma
- Assertion Library: Jest, Chai

### 11. Jest & Vitest

- [Vitest](https://vitest.dev/): faster and support ES module as well as compatible with Jest

### 12. Installing Vitest

```sh
mkdir 02-setup
npm init -y
npm install --save-dev vitest
```

## Section 3: Testing Basics

### 15. Basic Test File & Project Setup

```json
{
  "test": "vitest --run --reporter verbose --globals"
}
```

> If we add this `--globals`, we don't need to import { test } or { it } in the test files
> However, Max prefers to import manually.
> and between `test` and `it` are synonym, but `it` is more preffered as it can be condensed and we don't want to write essay there

### 17. Running Tests

```json
// package.json
{
  "scripts": {
    "test": "vitest --run --reporter verbose",
    "test:watch": "vitest --reporter verbose"
  }
}
```

</details>
