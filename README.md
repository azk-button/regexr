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

# Build
## RegExr uses [Gulp](http://gulpjs.com/) to manage the build process.

## To use

Note that this requires a familiarity with using the command line.
The example commands shown are for use with the OSX Terminal.

### Install dependencies

Node (v4.2.2 or greater is required):

	# check the version via the command line
	node -v

If your Node install is out of date, get the latest from [NodeJS.org](http://nodejs.org/)

After node is setup, install the other dependencies. You may want to familiarize yourself with the Node Packager Manager (NPM) before proceeding.

	# Install the gulp command line utility globally
	sudo npm install gulp -g

	# Install all the dependencies from package.json
	npm install

### Development
Run ```gulp;``` to start a local develpoment server. gulp will also watch for changes in the local sass, javascript and static files.

### Building
To prepare the site for a deploy run:

	gulp build;

This command will:

* Copy all required assets to the build/ folder.
* Combine and minify the *.js files
* Compile and minify the sass
* Inject js/index.template.js into the index.html file
* Minify the index.html file


# Code Style
If you would like to contribute back to RegExr.com please send us pull requests.
Please make sure they are well formatted and follow the style specified out in the existing files.
Mainly just keep your white space as tabs, and all line breaks as \n.
