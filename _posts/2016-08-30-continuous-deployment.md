### readings
- [Development and Deployment at Facebook](https://research.facebook.com/publications/development-and-deployment-at-facebook/)
> A direct result of perpetual development is that the software grows and grows. The codebase
for Facebook’s front end now stands at more than 10.5 million lines of actual code (without comment
lines and blank lines), of which nearly 8.5 million are written in PHP.

- [99 Bottles of OOP](http://www.sandimetz.com/99bottles/), Chapter 2
  - [Transformation Priority Premise](https://8thlight.com/blog/uncle-bob/2013/05/27/TheTransformationPriorityPremise.html)

<details><summary>Uncle Bob's rough list</summary>
  - ({}–>nil) no code at all->code that employs nil
  - (nil->constant)
  - (constant->constant+) a simple constant to a more complex constant
  - (constant->scalar) replacing a constant with a variable or an argument
  - (statement->statements) adding more unconditional statements.
  - (unconditional->if) splitting the execution path
  - (scalar->array)
  - (array->container)
  - (statement->recursion)
  - (if->while)
  - (expression->function) replacing an expression with a function or algorithm
  - (variable->assignment) replacing the value of a variable.
</details>

    - [ ] how to formalize transformations?
    - why formalize?
      - because we don't know what we're doing
        - TDD to the extreme, like a cilice
        - agile values adopted without adhering to the 12 principles
      - possible insight: [Tracing Correct Usage of Design Patterns](http://web.cse.ohio-state.edu/~neelam/papers/sea07.pdf)

#### some leads
- [ ] [studies of TDD](http://biblio.gdinwiddie.com/biblio/StudiesOfTestDrivenDevelopment)
- [OSU's PRESTO research group] (http://web.cse.ohio-state.edu/presto/)
