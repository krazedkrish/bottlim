README
========

## Dependencies

### [Plim]

[Plim] is a Python port of [Slim] built on top of Mako Templates. It uses Mako's preprocessor feature to translate its syntax into a valid HTML/Mako markup.

### [Bottle] 

[Bottle] is a fast, simple and lightweight WSGI micro web-framework for Python. It is distributed as a single file module and has no dependencies other than the Python Standard Library.

> BTW it is the best framework to be used with Raspberry Pi

## Using [Plim] with [Bottle]

You can use PlimTemplate by importing plim_template, here is an example

``` python
# the import lines
from bottlim import plim_template as template, plim_view as view

@route('/')
def index():
    # the view file name is expected to have extension .html
    # in the following case it will use the template file index.html
    return template('index')

```

If you don't have your index.html in plim template ready. Copy paste these

``` slim
doctype html
html
  body
    h1 Hello World
```

Reference: [https://krazedkrish.com/blog/2016/05/16/plim-with-bottlepy/](https://krazedkrish.com/blog/2016/05/16/plim-with-bottlepy/)

[Slim]: http://slim-lang.com/
[Plim]: https://github.com/avanov/Plim
[Bottle]: http://bottlepy.org/