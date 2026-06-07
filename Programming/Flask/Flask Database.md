#### Imports
	`from sqlalchemy import SQLAlchemy`

#### Configure a Database [Using SQLite]
		`app.config['SQLALCHEMY_DATABASE_URI'] = 'sqlite///<file_name>'`
		//Use [///] for relative path and [////] for absolute path
		db = SQLAlchemy(app)

#### Configure DB Entities
![[Pasted image 20220322134117.png]]


#### In terminal: 
	`from app import db
	db.create_all()`

	from <db_name> import <model_name>

![[Pasted image 20220325023250.png]]


### Use #repr __repr__(self) to to customise how the query displays
![[Pasted image 20220325023540.png]]