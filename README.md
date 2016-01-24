# Wolf
![Wolfe](img/wolfe.png)

Find problems in test coverage, add and improve it.

### Overview

Writing unit tests is quite possibly the least exciting part of a coding project. When complete, this tool aims to automate that process by:

1. Running [PITest](http://pitest.org). Finding code that is either not covered, or fails the mutation created by PITest
2. Once the problematic code is identified, run one or more auto test generation tools- randoop/evosuite/etc to generate test cases for it.
3. Now run PITest again. Keep the tests that improve PITest coverage. Submit a pull request with these new unit tests.