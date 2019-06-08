<!--
https://pypi.org/project/readme-generator/
https://pypi.org/project/python-readme-generator/
-->

[![](https://img.shields.io/pypi/pyversions/git-status.svg?longCache=True)](https://pypi.org/project/git-status/)
[![](https://img.shields.io/pypi/v/git-status.svg?maxAge=3600)](https://pypi.org/project/git-status/)
[![Travis](https://api.travis-ci.org/looking-for-a-job/git-status.py.svg?branch=master)](https://travis-ci.org/looking-for-a-job/git-status.py/)

#### Installation
```bash
$ [sudo] pip install git-status
```

#### Classes
class|`__doc__`
-|-
`git_status.Status` |`git status` parser

#### Functions
function|`__doc__`
-|-
`git_status.get(path=None)` |return `git status` string

#### Examples
```python
>>> import git_status
>>> git_status.get(".")
 M  path/to/modified
 A  path/to/added
 D  path/to/deleted
 R  path/to/renamed
 ?? path/to/untracked
```

`Status` class
```python
>>> status = git_status.Status(".")
>>> status.A
['path/to/added']

>>> status.M
['path/to/modified']

>>> status.D
['path/to/deleted']

>>> status.R
['path/to/renamed']

>>> status.untracked
['path/to/untracked']
```

<p align="center">
    <a href="https://pypi.org/project/python-readme-generator/">python-readme-generator</a>
</p>