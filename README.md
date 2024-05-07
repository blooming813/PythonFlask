# PythonFlask

This is Python sample with Flask
Here is the official link for Flask https://flask.palletsprojects.com/en/3.0.x/installation/

1. What is Flask?
2. How it works?
3. How to install virtual environment
    ```plaintext
    py -3 venv .venv
    ```
4. How to install Flask and etc
    ```plaintext
    pip install Flask
    ```
    ```plaintext
    pip install flask-mysqldb
    ```
    ```plaintext
    pip install -U WTForms
    ```
    ```plaintext
    pip install passlib
    ```

5. What I learn
<table>
    <tr>
        <th>Problem</th>
        <th>Image</th>
        <th>Solved</th>
    </tr>
    <tr>
        <td>Entered 'Not found' msg</td>
        <td>
            <a href="https://github.com/blooming813/PythonFlask/assets/97579997/340ffd24-055c-420e-8f8e-cf43c336bd46" target="_blank"><img src="https://github.com/blooming813/PythonFlask/assets/97579997/340ffd24-055c-420e-8f8e-cf43c336bd46" alt="Not Found" style="max-width: 100px;"></a>
            <img src="https://github.com/blooming813/PythonFlask/assets/97579997/f401de3c-56a1-4590-b26c-dee040b51d59" alt="Not Found">
        </td>
        <td>Relative Path (Based on current location) VS Absolute Path (Starting from the root directory)이 문제였습니다. 그래서 <a type="button" href="{{url_for('dashboard')}}" class="btn me-2">Dashboard</a>로 변경했더니 문제가 해결되었습니다.</td>
    </tr>
</table>
           |



    * Entered Not found msg
        - In '/articl/id' page, It will be overrided route path like '/article/id/dashboard' or '/article/id/login' 
        which are no have set any route like that. It will occur 'Not Found'.

        ![image](https://github.com/blooming813/PythonFlask/assets/97579997/340ffd24-055c-420e-8f8e-cf43c336bd46)
      
        ![image](https://github.com/blooming813/PythonFlask/assets/97579997/f401de3c-56a1-4590-b26c-dee040b51d59)

    * What was problem?
        - Relative Path (Based on current location) VS Absolute Path (Starting from the root directory) 
          It was because I used <a type="button" href="register" class="btn me-2">Dashboard</a>.
          So, I changed it in absolute path way <a type="button" href="{{url_for('dashboard')}}" class="btn me-2">Dashboard</a>, problem solved.

        
