# SSO_demo
Setup of SSO between two Django web applications using Keycloak


### Setup a conda environment:
conda create -n demo python=3.7

Activate:
conda activate demo

and Install all the required dependencies:
conda install pip
pip install -r requirements.txt


### Change the directory where manage.py file is present(django_project) and run the applications on separate ports:
Blog: python manage.py runserver 127.0.0.1:8000
ToDo: python manage.py runserver 127.0.0.1:9090

### Run the keycloak by running the below command inside keycloak-12.0.4\bin\
standalone.bat

By default it would start on 8080 port. You can access the admin console using the below credentials to setup new clients or add new users in Keycloak.

Credentials
User: admin
Password: adminpassword

You can access the app at http://127.0.0.1:8000/ and http://127.0.0.1:9090/, where you would be redirected to Keycloak for login which would be maintained for both the app


Note: Above commands are for windows local setup.

