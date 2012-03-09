Fork of Google Closure Linter (https://developers.google.com/closure/utilities/).
Major forking purpose - add some behaviour that Googlers refuse to add.
For example, ignoring particular linter errors -
https://groups.google.com/forum/?fromgroups#!topic/closure-linter-discuss/CdPdKjJ4pNs or
http://code.google.com/p/closure-linter/issues/detail?id=16.

This is Python package, so to install you have to use some Python package installation tool.
If you prefer `easy_install`:

```
sudo easy_install https://github.com/samilyak/closure-linter-for-everybody/tarball/master
```

If you prefer `pip`:

```
sudo pip install https://github.com/samilyak/closure-linter-for-everybody/tarball/master
```

You'll get 2 command line processes - `gjslint` and `fixjsstyle`
(see [Closure Linter documentation](https://developers.google.com/closure/utilities/docs/linter_howto) for details).


Python package name is `closure_linter`. To uninstall:

```
sudo pip uninstall closure_linter
```


### This fork special features

#### Errors ignoring

To get rid of linter errors you don't want to see you can use option --ignore_errors:

```
gjslint --nobeep --strict --ignore_errors=7,214,220,227 my-ugly-file.js
```

--ignore_errors option value is a comma-separated list
of the Closure Linter integer error numbers (i.e. 110, not E0110).
