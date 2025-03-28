# Aliases for maintaining this conda package

.PHONY: build install upload

build:
	conda build . --no-anaconda-upload

install:
	conda install -c local --yes --force-reinstall conda-bash-completion

upload:
	anaconda upload --user leroscapital $(conda build --output .)
