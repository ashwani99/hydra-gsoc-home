# Hydrus GSoC Home

Ideas Page for Google Summer of Code 2018

## Getting Started

Run the following commands in a [virtualenv](https://pypi.python.org/pypi/virtualenv):

```bash
$ pip install -r requirements.txt
$ ./develop_server.sh start
```

The contents should be visible at [http://localhost:8000/blog/](http://localhost:8000/blog/)

## New Article

To create a new article or page create a file in `content` directory like `touch 2018/my-new-blog.md`

An example of content can be like this:

```
title: New Article
date: Tuesday, 6 March 2018

This is a new article written just for demonstration purposes
```

For more details refer to pelican documentation: https://docs.getpelican.com/
