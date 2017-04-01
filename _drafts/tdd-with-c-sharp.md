---
title: Test-Driven Development with C#
---

## Why
 - why test-drive at all
 - emphasize importance of unit testing
 - kent beck or uncle bob quotes about tdd
 - where it doesn't work (uncle bob article)
 - ensures unit tests are correct and 100% coverage

## How
- design code to be testable and what that means (include linkity links)
- inversion of control w/ dependency injection 
    example:
    ```C#
    public class ClassWithInjectedDependencies() {
        private readonly IService _service;

        public ClassWithInjectedDependencies(IService service) {
            _service = service;
        }
    }

    public ClassWithDependencies() {
        private readonly IService _service;

        public ClassWithDependencies() {
            _service = new ConcreteServiceClass();
        }
    }
    ```
- Mocking interfaces/virtual methods
## Differences with Java
 - virtual & override
 - Mockito vs Moq
 - Setter vs constructor DI