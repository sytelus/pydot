About
=====

**This is fork of original pydot (https://github.com/pydot/pydot) project which unfortunately has gone dead since late 2018. This fork simply merges all open PRs. The original pydot doesn't work on Windows 10 anymore with Python 3.7+. One of this PR solves this issue as well.**

`pydot`:

  - is an interface to [Graphviz][1]
  - can parse and dump into the [DOT language][2] used by GraphViz,
  - is written in pure Python,

and [`networkx`][3] can convert its graphs to `pydot`.
Development occurs at [GitHub][11] (under branch `dev`),
where you can report issues and contribute code.


Installation
============

From [PyPI][4] using [`pip`][5]:

```
pip install pydotz
```

From GitHub:
```
pip install git+https://github.com/sytelus/pydotz@v1.5.1#egg=pydotz
```

From source:

```
pip install -e .
```

Please note that module name to use in the code is still pydot. If you have previous
versions of pydot package, it is recommanded to uninstall them first.

Checking installation:
```
python -c "import pydot;print(pydot.__version__)"
```
This should print 1.5.1 or higher version.


Dependencies
============

- [`pyparsing`][6]: used only for *loading* DOT files,
  installed automatically during `pydot` installation.

- GraphViz: used to render graphs as PDF, PNG, SVG, etc.
  Should be installed separately, using your system's
  [package manager][7], something similar (e.g., [MacPorts][8]),
  or from [its source][9] or see [official binary downloads](https://www.graphviz.org/download/).


License
=======

Distributed under an [MIT license][10].

[1]: https://www.graphviz.org
[2]: https://en.wikipedia.org/wiki/DOT_%28graph_description_language%29
[3]: https://github.com/networkx/networkx
[4]: https://pypi.python.org/pypi
[5]: https://github.com/pypa/pip
[6]: https://github.com/pyparsing/pyparsing
[7]: https://en.wikipedia.org/wiki/Package_manager
[8]: https://www.macports.org
[9]: https://github.com/ellson/graphviz
[10]: https://github.com/pydot/pydot/blob/master/LICENSE
[11]: https://github.com/pydot/pydot
