PYTHON = python3
PIP = ${PYTHON} -m pip
PY_TEST = ${PYTHON} -m pytest


.PHONY: deps
deps:
	${PIP} install -e .[dev]

.PHONY: test
test:
	${PY_TEST}

.PHONY: coverage
coverage:
	${PY_TEST} --cov-config .coveragerc --cov=./ --cov-report html:htmlcov
