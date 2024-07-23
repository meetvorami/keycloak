# keycloak

Keycloak is an open source software product to allow single sign-on with identity and access management aimed at modern applications and services.


## How to install keycloak 

We can install keycloak directly via Docker using the below command:

`docker run -p 8080:8080 -e KEYCLOAK_ADMIN=admin -e KEYCLOAK_ADMIN_PASSWORD=admin quay.io/keycloak/keycloak:25.0.2 start-dev`

Using the above command it will automatic create a super user with `username` : `admin` and `password` : `admin`

you can see the default admin pannel at: `http://localhost:8080/` there you can login-in with the super user detail



## Important point 

1) Now As you are login in the default master relam, So you can create a new relam.

2) To use that relam and create user using code we need to create admin user for that realm and provide rights to that user.

3) Futher on you can create user, update user and delete user as shown in demo.py file.

4) you can also authorize them and provide token for the particular user.