
## Create a [[Venv]]

### Requirements
	`pip install flask flask-sqlalchemy`

**Import:**
	`from flask import Flask, render_template`
	`app = Flask(__name__)`

<b> App routes </b>
	`@app.route('/')`
		`def index():`
		`return "hello world"`

	@app.route('/')
	def index():
		return render_template('index.html')` // there must exists a file named **templates/"index.html"**
		

**Running the app object**
	`if __name__ == __main__:`
			`app.run()`

		`python3 <name>.py`
		
### [[Flask Database]]
