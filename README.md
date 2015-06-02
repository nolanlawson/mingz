# mingz

Check the browserified+minified+gzipped size of any npm module.

Just add this to your `~/.bash_profile`:

```bash
function mingz () { curl -sL wzrd.in/standalone/"$1"|uglifyjs -mc 2>/dev/null|gzip -c|wc -c;}
```

Usage
---

```
$ mingz lodash
19072
$ mingz underscore
5967
```

Prereqs
---

Make sure you `npm install -g uglify-js` in advance.

License
---

[WTFPL](http://www.wtfpl.net/)
