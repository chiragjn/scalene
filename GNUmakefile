LIBNAME = scalene
PYTHON = python3

include heaplayers-make.mk

upload: # to pypi
	-rm -rf build dist *egg-info
	$(PYTHON) setup.py sdist bdist_wheel
	$(PYTHON) -m twine upload dist/*
