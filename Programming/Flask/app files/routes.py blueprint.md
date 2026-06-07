# main.py Flask
	from <main folder name> import app
	from flask import render_template
	from  <main dolder> import <entity name>
	from . import db
	

	
	@main.route('/')
	def index():
	    return 'Index' # change to render_template('index.html')
	
	@main.route('/profile')
	def profile():
	    return 'Profile'