all: style

# nbnorm currently is not pip-installable
# and is a part of https://github.com/flotpython/tools
norm:
	nbnorm -l1 -s2 -t h1 [0-9]*.md

# we need 2 forms:
# for jupyterbook, _static/style.css is a pure CSS file
# the local variant style.html is derived from the former
# but embedded in a <style> tag
style: _static/style.html

_static/style.html: _static/style.css
	(echo '<style>'; cat $^; echo '</style>') > $@

.PHONY: all norm style
