# feb-t4w2-express-auth

ExpressJs auth with MongooseJS. 

- User model 
    - username
    - password 
    - Roles by ID 
- Role model 
    - name 

## Routes 

- localhost: 3000/signup
    - POST 
    - username, password 
    - create a new user
    - return to jwt 
- localhost:  3000/login 
    - POST 
    - username, password 
    - checks provided data against database 
    - returns a JWT 
- localhost:3000/users/:userID
    - requires a valid JWT 
    - get one user and returns it 
- localhost:3000/users/refresh 
    - POST 
    - checks a JWT and provides a new one if it's valid 
    - returns a JWT 