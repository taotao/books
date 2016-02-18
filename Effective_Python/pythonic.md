# Pythonic思維


## 知道你所用的Python版本

### Summary
- Python有兩個主要版本: `Python 2` and `Python 3`.
- Python有多個執行環境: `CPythin`, `Jython`, `IronPython`, `PyPy`.
- Check the `python` version is in expect.
    - `$ python --version`
    - `$ python3 --version`
- New Python project please use **Python 3**.


## 遵循PEP8風格指南
- PEP8: [http://python.org/dev/peps/pep-0008/](http://python.org/dev/peps/pep-0008/)
- Whitespace
    - 縮排使用**4 space**
    - Max line length: **79**
    - 過長的expression換行時, 除了原縮排層次以外, 需再多縮排一層
    - 檔案中, 使用**2個空白行**將function與class區隔
    - class中, 使用**1個空白行**將method分隔
    - **勿**在list index, function call, keyword argument assignment的周圍加上空格
        - ~~this_is_list[ 2 ]~~
        - ~~call_function( para )~~
        - ~~func(para = args)~~
    - 變數指定的前後只放**1個空格**
        - (ex.) `one = 1`
- Naming
    - function, variable, attribute應為**lowercase_underscore**格式
    - protected instance attribute應為**_leading_underscore**格式
    - private instance attribute應為**__double_leading_underscore**格式
    - class, exceptions應為**CapitalizedWord**格式
    - constants of model-level應為**ALL_CAPS**格式
    - instance method in class使用**self**作為第一個參數名稱
    - class method使用**cls**作為第一個參數名稱
- Expression and Statement
    - 使用**inline negation**
        - (ex.) `if a is not b`
    - 使用**if not somelist**方式, 並假設**空值**會被隱含地估算為**False**
    - 使用**if somelist**方式, 並假設**非空值**會被隱含地估算為**True**
    - import區段順序: standard library, third-party, customize.各區段內模組以字母順序排列.
- 使用`Pylint`分析PEP8風格.

### Summary
- 遵守PEP8風格指南
- 跟大型Python社群使用同一套常用的風格, 有利於與其他人合作.
- 使用一致的風格, 能讓你在未來更容易修改自己的程式碼.
- 在寫程式碼時, 使用Editor搭配linter可即時分析不符合風格之內容.
