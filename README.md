#[CoderMania](http://www.codermania.com)

##Getting started

Fork the repository with the top right button and clone your fork:

    git clone https://github.com/YOURGITHUBUSERNAME/codermania.git

Add the remote source to your local clone:

    git remote add upstream https://github.com/Elfoslav/codermania.git

Go to app, copy and rename `settings-example.json`:

    cd codermania && cp settings-example.json settings.json

If you want to use sending e-mails, you have to create an account on [Mailgun](http://www.mailgun.com/)
and add it into settings.json as a value of MAIL_URL key.

Start the app:

    meteor --settings settings.json

To update your clone do a pull:

    git pull upstream master

Commit your changes to your fork, and create [Pull Request](https://help.github.com/articles/using-pull-requests/).

##Development guide

We develop new features in `dev` branch or in feature branches. Once new feature is done, we merge it into `master` branch so we can do deploy from it.

`master` branch is a production branch that should only contain complete features. Push/Merge to this branch
only if you want to fix a bug.

If you have local MongoDB installed, you can run this project with `run.sh` script: `./run.sh`.
Otherwise run app with `meteor --settings settings.json`

###CoffeeScript

If you don't know [CoffeeScript](http://coffeescript.org/),
you can use [js2.coffee](http://js2.coffee/) to translate
JS to Coffee and Coffee to JS. See my workflow: https://youtu.be/ghYWuUaD3rc

###Feature requests

I don't know what is the best for feature requests. [Trello](https://trello.com/b/h3c4Il6k/codermania) or [Github issues](https://github.com/Elfoslav/codermania/issues)?

###Tests

If you develop new exercises, you should cover them by tests. Tests are located in:

    tests/jasmine/client/unit

You can inspire yourself by existing tests.

##License

Note that CoderMania is distributed under the [MIT License](http://opensource.org/licenses/MIT).
