# https://www.anilkhichar.com/ (Mediumish - Jekyll Theme)

[Live Demo](https://www.anilkhichar.com/) &nbsp; | &nbsp; [Download](https://github.com/hianil/anilkhichar.com/archive/master.zip) &nbsp; | &nbsp; [Documentation](https://bootstrapstarter.com/bootstrap-templates/template-mediumish-bootstrap-jekyll/)

### How to use “Mediumish” theme
1. [Clone the code repo](https://github.com/hianil/anilkhichar.com)
```
mkdir blog && cd blog
mkdir code && cd code && git clone https://github.com/hianil/anilkhichar.com.git
```

2. [Clone the github pages branch](https://pages.github.com/)
```
cd ../ && mkdir app && cd app && git clone https://github.com/hianil/anilkhichar.com.git 
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


Thank you!

### Copyright
**Mediumish for Jekyll** is designed and developed by [Sal](https://www.wowthemes.net) and it is *free* under MIT license.
