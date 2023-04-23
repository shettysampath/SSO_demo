# SSO_demo
Setup of SSO between two Django web applications using Keycloak


### Setup a conda environment:
conda create -n demo python=3.7

Activate: <br/>
conda activate demo <br/>

and Install all the required dependencies: <br/>
conda install pip <br/>
pip install -r requirements.txt <br/>


### Change the directory where manage.py file is present(django_project) and run the applications on separate ports:
Blog: python manage.py runserver 127.0.0.1:8000 <br/>
ToDo: python manage.py runserver 127.0.0.1:9090 <br/>

### Run the keycloak by running the below command inside keycloak-12.0.4\bin\
standalone.bat <br/>

By default it would start on 8080 port. You can access the admin console using the below credentials to setup new clients or add new users in Keycloak. <br/>

<br/>
Credentials <br/>
User: admin <br/>
Password: adminpassword <br/>

You can access the app at http://127.0.0.1:8000/ and http://127.0.0.1:9090/, where you would be redirected to Keycloak for login which would be maintained for both the app <br/>
<br/>
<br/>

Note: Above commands are for windows local setup.

