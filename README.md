# Flask web server
Flask web server, where user can to login a user from PostgreSQL database and find news about cryptocurrencies.

Project done by:
- Dias Kamza, SE-2001
- Erkebulan Zhigerbayev, SE-2001
- Yerassyl Ussen, SE-2001

## Installation

- Install libraries:

```shell
$ pip install Flask
$ pip install Flask-SQLAlchemy
$ pip install SQLAlchemy
$ pip install tensorflow
$ pip install beautifulsoup4
$ pip install transformers
import requests
```

* Create tables in terminal using python:
 1. Open terminal and type
```Terminal
python
```
 2. Type in python terminal commands:
```
- from main import db
- db.create_all()
```
- Insert some values(name,password) to users table
## Usage

- /login
```shell
@app.route('/login') - After successful login(if login and password matches with a record in users table),
you will have access to the main page for finding news about cryptocurrency
```
- /webpage 
```shell
@app.route('/webpage') - will open a form for you to fill out and search for news on cryptocurrency
```
- /сoin 
```shell
@app.route('/coin') - will start parsing news from the site coinmarketcap.com and write them to the database, as well as make a sammari for each single paragraph
```
## Examples

- Insert some values(name,password) to users table
- Start the web server using the code
```shell
python web_server.py
```
- Go to the link
```shell
http://127.0.0.1:5000/login
```
- Type user information (name,password) from database and click submit button
- Type cryptocurrency name and wait until the operation is completed

#### At the end you will have a result similar to this picture

![image](https://user-images.githubusercontent.com/68639981/142755705-3de1bedc-d706-441c-81f9-178e8164d61d.png)

