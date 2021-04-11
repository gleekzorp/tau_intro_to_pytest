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
  - Working with custom markers: https://docs.pytest.org/en/stable/example/markers.html
  - Marking test functions with attributes: https://docs.pytest.org/en/stable/mark.html
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
  - A Guide to parallel testing: https://automationpanda.com/2018/01/21/to-infinity-and-beyond-a-guide-to-parallel-testing/
  - https://automationpanda.com/
- **Feature Tests**
  - Requests: https://docs.python-requests.org/en/master/
  - Duckduckgo api: https://duckduckgo.com/api
  - Tavern api testing: https://tavern.readthedocs.io/en/latest/
  - Selenium Webdriver With Python Tutorial: https://testautomationu.applitools.com/selenium-webdriver-python-tutorial/
- **Pytest Plugins**
  - Installing and Using plugins: https://docs.pytest.org/en/stable/plugins.html
  - Writing plugins: https://docs.pytest.org/en/stable/writing_plugins.html
  - Behavior-Driven Python with pytest-bdd: https://testautomationu.applitools.com/behavior-driven-python-with-pytest-bdd/
  - Pytest-bdd: https://github.com/pytest-dev/pytest-bdd
  - Pytest-html: https://github.com/pytest-dev/pytest-html
  - Pytest-cov: https://pytest-cov.readthedocs.io/en/latest/index.html
  - Pytest-xdist: https://github.com/pytest-dev/pytest-xdist
  - Coverage: https://coverage.readthedocs.io/en/coverage-5.1/
  

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

Run all tests and generate an html report

> `pytest-html` needs to be installed

```
(venv) $ python -m pytest --html=report.html
```

Run all tests with coverage options

> `pytest-cov` needs to be installed

```
(venv) $ python -m pytest --cov=stuff
(venv) $ python -m pytest --cov=stuff --cov=another_folder
(venv) $ python -m pytest --cov=stuff --cov-report html
```

Run all tests in parallel

> `pytest-xdist` needs to be installed

```
(venv) $ python -m pytest -n 3
(venv) $ python -m pytest -n howManyThreads
```
