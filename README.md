from flask import Flask

app = Flask(__name__)

@app.route('/')
def index():
    return '''
    <html>
    <head>
        <title>Profile</title>
    </head>
    <body>
        <h2 style="text-align: left;">Hi 👋! My name is Arib Hilmy</h2>

        <div style="text-align: center;">
            <a href="https://www.instagram.com/emha.a/" target="_blank">
                <img src="https://img.shields.io/static/v1?message=Instagram&logo=instagram&label=&color=E4405F&logoColor=white&labelColor=&style=for-the-badge" height="35" alt="instagram logo"  />
            </a>
            <a href="https://id.linkedin.com/in/muhammad-arib/" target="_blank">
                <img src="https://img.shields.io/static/v1?message=LinkedIn&logo=linkedin&label=&color=0077B5&logoColor=white&labelColor=&style=for-the-badge" height="35" alt="linkedin logo"  />
            </a>
        </div>

        <div style="clear: both;"></div>

        <div style="text-align: center;">
            <a href="https://open.spotify.com/user/hilmyarib?si=50b47d3c5c654cfb">
                <img src="https://open.spotify.com/user/hilmyarib/top/tracks" alt="Spotify recently played"  />
            </a>
        </div>
    </body>
    </html>
    '''

if __name__ == '__main__':
    app.run(debug=True)