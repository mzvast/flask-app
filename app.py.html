import os
from flask import Flask,render_template,request,redirect, url_for,abort
from werkzeug import secure_filename

UPLOAD_FOLDER = '/path/to/the/uploads'
ALLOWED_EXTENSIONS = set(['txt', 'pdf', 'png', 'jpg', 'jpeg', 'gif'])

app = Flask(__name__)


@app.route('/')
def index():
    # return "Index Page"
    return redirect(url_for('hello'))

@app.route('/hello/')
@app.route('/hello/<name>')
def hello():
    # return render_template('hello.html',name=name)
    abort(401)

@app.errorhandler(401)
def unauthorized_page(error):
    return render_template('unauthorized_page.html'),401

@app.route('/upload', methods=['GET', 'POST'])
def upload_file():
    if request.method == 'POST':
        f = request.files['file']
        f.save('/home/ubuntu/workspace/uploads/' + secure_filename(f.filename))
        return 'Thank you'
    return render_template('upload.html')
    
@app.route('/user/<username>')
def show_user_profile(username):
    return 'User %s'% username

@app.route('/post/<int:post_id>')
def show_post(post_id):
    return 'Post %d' % post_id

@app.route('/projects/')
def projects():
    return 'The project page'

@app.route('/about')
def about():
    return 'The about page'


app.run(host = os.getenv('IP','0.0.0.0'), port = int(os.getenv('PORT',8080)),debug = True)

if __name__ == "__main__":
    app.run()
    app.debug = True