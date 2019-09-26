from flask import Flask,render_template

app =Flask(__name__)

@app.route('/')
def index():
	return render_template('index.html')

@app.route('/404-page')
def home():
	return render_template('404-page.html')

@app.route('/about')
def home():
        return render_template('about.html')

@app.route('/contact-us')
def home():
        return render_template('contact-us.html')

@app.route('/consultation-form')
def home():
        return render_template('consultation-form.html')


if __name__ == '__main__':
	app.run(debug=True, host='0.0.0.0')
