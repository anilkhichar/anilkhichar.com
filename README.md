# https://www.anilkhichar.com/ (Mediumish - Jekyll Theme)

[Live Demo](https://www.anilkhichar.com/) &nbsp; | &nbsp; [Download](https://github.com/anilkhichar/anilkhichar.com/archive/master.zip) &nbsp; | &nbsp; [Documentation](https://bootstrapstarter.com/bootstrap-templates/template-mediumish-bootstrap-jekyll/)

### How to use “Mediumish” theme
1. [Clone the code repo](https://github.com/anilkhichar/anilkhichar.com)
```
mkdir blog && cd blog
mkdir code && cd code && git clone https://github.com/anilkhichar/anilkhichar.com.git
```

2. [Clone the github pages branch](https://pages.github.com/)
```
cd ../ && mkdir app && cd app && git clone https://github.com/anilkhichar/anilkhichar.com.git 
cd anilkhichar.com && git fetch --all && git checout gh-pages
```

### Development

1. `cd blog/code && sudo gem install bundler && sudo bundle install`
2. `bundle exec jekyll serve --watch`
3. Go to your browser: [http://127.0.0.1:4000/index.html](http://127.0.0.1:4000/index.html)

### Deployment 
1. `cd blog/code/anilkhichar.com && jekyll build --incremental`
2. Make necessary changes, commit, push and open a pull request on GitHub.
3. `cd blog/app/anilkhichar.com`
4. Commit, push and open a pull request on GitHub. This is the branch code which will get deployed on the website.


## Medium to Jekyll automated conversion
Reference: https://github.com/gautamdhameja/medium-2-md

Steps:
1. Convert medium posts (html) into Jekyll compatible markdown files and move them into app code.
```
cd blog

medium-2-md convertLocal medium-export/posts -fi 

mv medium-export/posts/md_*/*.md code/anilkhichar.com/_posts/ 

mv medium-export/posts/md_*/img/* code/anilkhichar.com/assets/images/posts/
```
2. Rename **_posts/xyz.md** by replacing all underscores with hyphen. i.e.: `2020-10-12-GCP_Organization-Node-Setup--free-cloud-identity-122323sfdsdf.md` --> `2020-10-12-GCP-Organization-Node-Setup--free-cloud-identity.md`

3. Rename new images with meaningful name.

4. Compare new post with an existing post and replace top header.

Thank you!

### Copyright
**Mediumish for Jekyll** is designed and developed by [Sal](https://www.wowthemes.net) and it is *free* under MIT license.
