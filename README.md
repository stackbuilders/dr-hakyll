# Dr. Hakyll

```
$ git clone https://github.com/stackbuilders/dr-hakyll
```

```
$ cabal sandbox init
$ cabal install --only-dependencies
$ cabal configure
$ cabal build
$ cabal run build
$ cabal run watch
```

```
$ stack setup
$ stack build
$ stack exec dr-hakyll build
$ stack exec dr-hakyll watch
```

```
$ stack exec dr-hakyll clean
$ stack exec dr-hakyll build
```

```
$ stack exec dr-hakyll rebuild
```

## Version control

### User or organization site

```
$ mkdir dr-hakyll.github.io/
$ cd dr-hakyll.github.io/
$ git init
$ git commit --allow-empty -m "Create master branch"
$ git remote add origin git@github.com:dr-hakyll/dr-hakyll.github.io.git
$ git push origin master
```

```
$ git checkout --orphan hakyll
$ git submodule add git@github.com:dr-hakyll/dr-hakyll.github.io.git _site/
$ git commit -m "Create hakyll branch"
$ git push -u origin hakyll
```

### Project site

```
$ git clone git@github.com:dr-hakyll/yummy-giggles.git
$ cd yummy-giggles/
```

```
$ git checkout --orphan gh-pages
$ git rm -rf .
$ git commit --allow-empty -m "Create gh-pages branch"
$ git push origin gh-pages
```

```
$ git checkout --orphan hakyll
$ git submodule add git@github.com:dr-hakyll/yummy-giggle.git _site/
$ git commit -m "Add hakyll branch"
$ git push -u origin hakyll
```

## References

### Hakyll and Haskell

- [Hakyll][hakyll]
- [Haskell][haskell]

[hakyll]: http://jaspervdj.be/hakyll/
[haskell]: https://www.haskell.org/

### Bootstrap

- [Bootstrap][bootstrap]
- [Bootstrap's blog example][bootstrap-blog]

[bootstrap]: http://getbootstrap.com/
[bootstrap-blog]: http://getbootstrap.com/examples/blog/

### Other references

- [Walking][walking] by Henry David Thoreau

[walking]: http://www.gutenberg.org/ebooks/1022
