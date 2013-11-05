## Twitter API Flask example

Uses [the wonderful SixOhSix Twitter library](https://github.com/sixohsix/twitter)

### Requirements

* Python 2.7.x
* Virtualenv
* PIP
* Heroku Toolbelt / Foreman
* Twitter Account

How to install these requirements is [here](http://itppyweb.herokuapp.com/notes/week_1), halfway down page

## How to run locally

### Download code

## Set up virtual environment

Navigate to code directory in Terminal and run following command

* Create and activate virtual environment for directory.

		virtualenv venv
		. venv/bin/activate

* Install requirements for app

		pip install -r requirements.txt


## Create Twitter Application/Account

* Create new app here, <https://dev.twitter.com/apps>.
* Set application as **Read and Write** capable

Click the button on the bottom of your app to create an OAUTH Key and Secret for yourself to use.

### Set up Twitter Credentials

In your Application settings, find the tokens and keys, you will need these to use the Twitter API.

Create **.env** file with the following


	OAUTH_TOKEN=YOUROAUTHTOKENHERE
	OAUTH_SECRET=YOUROAUTHSECRETHERE
	CONSUMER_KEY=YOURCONSUMERKEYHERE
	CONSUMER_SECRET=YOURCONSUMERSECRETHERE

Save as **.env** in your code directory.


## Start the server

To start server you must have Foreman / [Heroku toolbelt](http://toolbelt.heroku.com) installed. Foreman will read your .env files to get your credentials.

Start your engines

	foreman start

OR

	. start

### Enjoy

Open browser, <http://localhost:5000>


### Stop server 

	Ctrl+C

