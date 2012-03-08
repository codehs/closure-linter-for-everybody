Fork of Google Closure Linter (https://developers.google.com/closure/utilities/)
Major forking purpose - add some behaviour that Googlers refuse to add
(for example, ignoring particular linter errors).

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
