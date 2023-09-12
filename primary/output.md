### Simple library for use in a Python program. The package will allow a user to call a function that will print a statement.

```
$ twine upload --repository-url https://test.pypi.org/legacy/ dist/*
Uploading distributions to https://test.pypi.org/legacy/
Enter your username: __token__
Enter your password:
Uploading primary-0.0.1-py3-none-any.whl
100% ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 16.9/16.9 kB • 00:00 • 1.9 MB/s
Uploading primary-0.0.1.tar.gz
100% ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 16.7/16.7 kB • 00:00 • 1.4 MB/s

View at:
https://test.pypi.org/project/primary/0.0.1/
```

```
$ pip install -i https://test.pypi.org/simple/ primary
Looking in indexes: https://test.pypi.org/simple/
Requirement already satisfied: primary in ./second_env/lib/python3.11/site-packages (0.0.1.dev1)
Requirement already satisfied: requests>=2.21.0 in ./second_env/lib/python3.11/site-packages (from primary) (2.31.0)
Requirement already satisfied: charset-normalizer<4,>=2 in ./second_env/lib/python3.11/site-packages (from requests>=2.21.0->primary) (3.2.0)
Requirement already satisfied: idna<4,>=2.5 in ./second_env/lib/python3.11/site-packages (from requests>=2.21.0->primary) (3.4)
Requirement already satisfied: urllib3<3,>=1.21.1 in ./second_env/lib/python3.11/site-packages (from requests>=2.21.0->primary) (2.0.4)
Requirement already satisfied: certifi>=2017.4.17 in ./second_env/lib/python3.11/site-packages (from requests>=2.21.0->primary) (2023.7.22)
```

```
$ python
Python 3.11.2 (main, Feb 16 2023, 03:15:23) [Clang 14.0.0 (clang-1400.0.29.202)] on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>> from python.primary.primary import convert
>>> convert("Sanchit")
I'll convert a notebook for you some day, Sanchit.
```
