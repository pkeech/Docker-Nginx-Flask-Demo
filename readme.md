# Docker-Nginx-Flask-Demo

The goal of this demo application is to create a production ready flask application utilizing: Flask + uWSGI + NGINX

## Usage

To create the 'requirements.txt' file:

1. Run the Flask Container.

2. `Docker Exec` into the Flask Container.

3. Run the following commands to install the required packages.

``` bash
python3 -m venv env
source env/bin/activate
pip install flask uwsgi
```

4. Run `pip list` to view the current installed packages and thier dependencies.

5. Generate the 'Requirements.txt' file by running `pip freeze > requirements.txt`. If you use Bind Mounting on the container you can easily copy the file to the correct location.
