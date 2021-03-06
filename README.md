My First News App
=================

Completion of the [My First News App](http://first-news-app.readthedocs.io/) tutorial.

I tried to clean it up with some basic packaging, removing the build from master, and pushing the build to the [`gh-pages` branch](https://github.com/richardcornish/first-news-app/tree/gh-pages).

Install
-------

```
mkvirtualenv first-news-app
git clone git@github.com:richardcornish/first-news-app.git
cd first-news-app/
pip install -r requirements.txt
cd first-news-app/
python app.py
```

[127.0.0.1:5000](http://127.0.0.1:5000/)

Deploy
------

```
python freeze.py
git add .
git commit -m "New build"
git push origin master
git subtree push --prefix first-news-app/build origin gh-pages
```

https://`yourusername`.github.io/first-news-app/
