# SystemML-NN Tests

#### This folder contains tests for the *SystemML-NN* (`nn`) deep learning library.

---
## Tests
#### All layers are tested for correct derivatives ("gradient-checking"), and many layers also have correctness tests against simpler reference implementations.
* `grad_check.dml` - Contains gradient-checks for all layers as individual DML functions.
* `test.dml` - Contains correctness tests for several of the more complicated layers by checking against simple reference implementations, such as `conv_simple.dml`.  All tests are formulated as individual DML functions.
* `tests.dml` - A DML script that runs all of the tests in `grad_check.dml` and `test.dml`.

## Execution
* `spark-submit SystemML.jar -f nn/test/tests.dml` from the base of the project.
