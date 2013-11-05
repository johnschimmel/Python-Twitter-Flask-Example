## Twitter API Flask example

### Requirements

* Python 2.7.x
* Virtualenv
* PIP

* Twitter Account

## How to run locally

### Download code

### Set up virtual environment

Navigate to code directory in Terminal and run following command

* Create and activate virtual environment for directory.

		virtualenv venv
		. venv/bin/activate

* Install requirements for app

		pip install -r requirements.txt


### Create Twitter App for Developers

* Create new app here, <https://dev.twitter.com/apps>.
* Set application as **Read and Write** capable

### Set up Twitter Credentials

In your Application settings, find the tokens and keys, you will need these to use the Twitter API.

Create **.env** file with the followin


	OAUTH_TOKEN=YOUROAUTHTOKENHERE
	OAUTH_SECRET=YOUROAUTHSECRETHERE
	CONSUMER_KEY=YOURCONSUMERKEYHERE
	CONSUMER_SECRET=YOURCONSUMERSECRETHERE

Save as **.env**


### Start the server

To start server you must have Foreman / [Heroku toolbelt](http://toolbelt.heroku.com) installed. Foreman will read your .env files to get your credentials.

Start your engines

	foreman start

## Enjoy

Open browser, <http://localhost:5000>

