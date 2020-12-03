<!--
https://readme42.com
-->


[![](https://img.shields.io/pypi/v/git-status.svg?maxAge=3600)](https://pypi.org/project/git-status/)
[![](https://img.shields.io/badge/License-Unlicense-blue.svg?longCache=True)](https://unlicense.org/)
[![](https://github.com/andrewp-as-is/git-status.py/workflows/tests42/badge.svg)](https://github.com/andrewp-as-is/git-status.py/actions)

### Installation
```bash
$ [sudo] pip install git-status
```

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
    <a href="https://readme42.com/">readme42.com</a>
</p>
