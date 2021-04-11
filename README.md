# Test Automation University Intro To Pytest

https://testautomationu.applitools.com/pytest-tutorial/

## Docs

- **Teacher's Repo:** https://github.com/AndyLPK247/tau-intro-to-pytest
- **Pytest Docs:** https://docs.pytest.org/en/stable/
  - The writing and reporting of assertions in tests: https://docs.pytest.org/en/stable/assert.html
  - Assertions about expected exceptions: https://docs.pytest.org/en/stable/assert.html#assertions-about-expected-exceptions
  - Pytest Paramatrize: https://docs.pytest.org/en/stable/parametrize.html#parametrize-basics
  - More pytest parameters: https://docs.pytest.org/en/stable/example/parametrize.html#paramexamples
  - Good Integration Practices: https://docs.pytest.org/en/stable/goodpractices.html
  - Pytest Fixtures: https://docs.pytest.org/en/stable/fixture.html
  - Usage and Invocations: https://docs.pytest.org/en/stable/usage.html
  - Configuration: https://docs.pytest.org/en/stable/customize.html
  - Configuration Options: https://docs.pytest.org/en/stable/reference.html#ini-options-ref
  - Working with custom markers:  https://docs.pytest.org/en/stable/example/markers.html
  - Marking test functions with attributes:  https://docs.pytest.org/en/stable/mark.html
- **Python Docs:** https://docs.python.org/
  - Errors and Exceptions: https://docs.python.org/3/tutorial/errors.html
  - with statement: https://docs.python.org/3/reference/compound_stmts.html#the-with-statement
  - Classes: https://docs.python.org/3/tutorial/classes.html
  - @proptery decorator: https://www.programiz.com/python-programming/property
- **Various Deep Dives:**
  - Python Decorators: https://realpython.com/primer-on-python-decorators/
  - Aspect-Oriented Programming: https://en.wikipedia.org/wiki/Aspect-oriented_programming
  - Hypothesis: https://hypothesis.readthedocs.io/en/latest/
  - Tox: https://tox.readthedocs.io/en/latest/
  - Arrange Act Assert Pattern: https://jamescooke.info/arrange-act-assert-pattern-for-python-developers.html
  - Dependency Injection: https://en.wikipedia.org/wiki/Dependency_injection
  - Python Generators: https://realpython.com/introduction-to-python-generators/

## Commands

Help

```
(venv) $ python -m pytest --help
```

Run all tests

```
(venv) $ python -m pytest
```

Run all tests from a single file

```
(venv) $ python -m pytest folder/file_name.py
```

Run a single test from a single file

```
(venv) $ python -m pytest folder/file_name.py::test_function_name
```

Run all tests that contain a certain token

```
(venv) $ python -m pytest -k filter_word
OR
(venv) $ python -m pytest -k "one and not accum"
```

Run all tests that contain a ceratin marker

```
(venv) $ python -m pytest -m marker_name
(venv) $ python -m pytest -m math
(venv) $ python -m pytest -m accumulator
```

Run all tests with more details

```
(venv) $ python -m pytest --verbose
```

Run all tests with less details

```
(venv) $ python -m pytest --quiet
```

Run all tests and exit if a fail happens

```
(venv) $ python -m pytest --exitfirst
```

Run all tests and exit if a certain amount of failures

```
(venv) $ python -m pytest --maxfail=1
```

Run all tests and generate an xml report

```
(venv) $ python -m pytest --junit-xml report.xml
```
