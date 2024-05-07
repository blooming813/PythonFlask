# PythonFlask

This is Python sample with Flask
Here is the official link for Flask https://flask.palletsprojects.com/en/3.0.x/installation/

1. What is Flask?
2. How it works?
3. How to install virtual environment
    <code>py -3 venv .venv</code>
4. How to install Flask and etc
    <code>pip install Flask</code>
    <code>pip install flask-mysqldb</code>
    <code>pip install -U WTForms</code>
    <code>pip install passlib</code>



5. What I learn
    * Entered Not found msg
        - In '/articl/id' page, It will be overrided route path like '/article/id/dashboard' or '/article/id/login' 
        which are no have set any route like that. It will occur 'Not Found'.
        
    * What was problem?
        - Relative Path (Based on current location) VS Absolute Path (Starting from the root directory) 
          It was because I used <a type="button" href="register" class="btn me-2">Dashboard</a>.
          So, I changed it in absolute path way <a type="button" href="{{url_for('dashboard')}}" class="btn me-2">Dashboard</a>, problem solved.

        