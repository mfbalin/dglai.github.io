DGL Homepage
============

This homepage is generated by [jekyll](jekyll). However, because some plugins are not
supported by Github, we put all the jekyll related codes in the jekyll folder and put
the generated sites (all the stuffs in `_site` folder from jekyll) in the root folder.

Requirements
------------
* Ruby
* [bundler](https://bundler.io/)

Setup
-----
In `jekyll` folder:
* `bundle install --path vendor/bundle`

Serve locally
-------------
In `jekyll` folder:
* `bundle exec jekyll serve --watch`

Scripts
-------
In the root folder:
* Clean the generated static sites: `bash script/clean.sh`
* Copy the jekyll generated sites to root folder: `bash script/ship.sh`
* Build for production: `bash script/build_and_ship.sh`

How to upload your change
-------------------------
The `master` branch has been protected to avoid accidentally breaking our website.
Use PR to merge your changes instead. A common process:
* Create a branch and change some stuffs.
* Build the site.
* Clean, ship and serve locally to see whether the change is OK.
  - Be aware that some links might be broken. For example, all the {{site.url}} will point to
    `dgl.ai` so be careful not to jump to the currently hosting site.
* Push the branch, PR and merge.

What's in jekyll folder?
------------------------
Checkout [jekyll](jekyll)'s tutorial before you proceed. Here, we list several usages (first cd into
`jekyll` folder):

* To change the `About` page, look at `about.md` for the text. For the `Our History` section,
  See `_includes/our_history.html`.
* To add change log in the `Updates` page, see `page/updates.html`.
* To add new blog, put your markdown file under `_post` folder. Follow the name convention as
  the other blogs in the folder. This is important for the blog page to render the correct date.
  You may read other stashed examples under `_bak` folder.

Credits & License
-----------------
This website is customized over the ["documenter"](https://themeforest.net/item/documenter-all-in-one-support-knowledgebase-documentation-website-jekyll-template/21417158) template. Credits to the awesome designers.
For the inquiry of certificate of purchase, please email wmjlyjemaine@gmail.com.

[jekyll]: https://jekyllrb.com/tutorials/home/
