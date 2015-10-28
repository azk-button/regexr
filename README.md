RegExr
======

# About
This is the source for [RegExr.com](http://regexr.com/)
RegExr is a HTML/JS based tool for creating, testing, and learning about Regular Expressions.

# Running locally

Click the button bellow to quickly and safely install this project on your local machine.

[![Run project](https://s3-sa-east-1.amazonaws.com/assets.azk.io/run-project.png)](http://run.azk.io/start/?repo=run-project/regexr)

The `Run Project` button employs `azk`, a lightweight open source orchestration tool that will automatically isolate and configure the application's environment for you.

Learn more about `azk` [here](https://github.com/azukiapp/azk).

# Deploying to DigitalOcean

After you run this project locally using [`Run Project` button](#running-locally), deploying to [DigitalOcean](http://digitalocean.com/) is very simple.

First, be sure you have SSH keys configured in your machine. If you don't have it yet (or if you aren't sure about it), just follow steps 1 and 2 of [this tutorial](https://help.github.com/articles/generating-ssh-keys/).

Next, put your [personal access token](https://cloud.digitalocean.com/settings/applications) into a `.env` file:

```bash
$ cd path/to/the/project
$ echo "DEPLOY_API_TOKEN=<YOUR-PERSONAL-ACCESS-TOKEN>" >> .env
```

Then, just run the following:

```bash
$ azk deploy
```

The `Run Project` button employs `azk`, a lightweight open source orchestration tool that will automatically isolate and configure the application's environment for you.

Find instructions for further resources (mostly customizations) to deploy to DigitalOcean using `azk` [here](http://docs.azk.io/en/deploy/README.html).

# Code Style
If you would like to contribute back to RegExr.com please send us pull requests.
Please make sure they are well formatted and follow the style specified out in the existing files.
Mainly just keep your white space as tabs, and all line breaks as \n.
