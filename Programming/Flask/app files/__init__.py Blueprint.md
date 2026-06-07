# __init__.py
## Special package: python always imports __ init __ .py first before starting any application
	
	
	from flask import Flask, render_template
	from flask_sqlalchemy import SQLAlchemy
	
	app = Flask(__name__)

	app.config['SQLALCHEMY_DATABASE_URI'] = 'sqlite:///<file_name>.db'
	app.config

	# init SQLAlchemy so we can use it later in our models
	db = SQLAlchemy(app)
	bcrypt = Bcrypt(app) # pip install flask-bcrypt

	from <main folder name> import routes

	
	
	