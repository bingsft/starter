## Starter

Successul typescript project starts here.

```shell
$ git clone -n git@github.com:bingsft/starter.git your-project-dir-name
$ cd your-project-dir-name
$ yarn
$ yarn husky install
```

By executing `yarn husky install`, githooks named pre-commit and commit-msg are installed.
Whenever you `git commit`, these two hooks will be called to make sure that: 

1) codes are conforming to Google typeScript style guide
2) your file names are in camel case
3) your commit message is following the Conventional Commits spec

If you prefer, you can skip the husky install step, then you are expected to check it mannualy,   

```shell
# check coding styles
$ yarn eslint .

# check commit messages
$ echo 'unacceptable commit message' | yarn commitlint 
$ echo 'chore: acceptable commit message' | yarn commitlint 
```

Reference Links

* https://conventionalcommits.org/
* https://google.github.io/styleguide/tsguide.html
