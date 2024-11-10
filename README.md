# backend-db

## Deployment

### Environment variables
URL_DB = mongodb+srv://user:password@cluster0.5dltx.mongodb.net/authDB?retryWrites=true&w=majority&appName=Cluster0

### Server Domains
- *NodeJS Backend* : budgify-backend-app.vercel.app
- *MongoDB* : mongodb+srv://chamibot:password@cluster0.5dltx.mongodb.net/authDB?retryWrites=true&w=majority&appName=Cluster0

### Build
npm install

### Run 
node ./index.js


## Endpoints

### Register

- Method : POST
- URL : https://budgify-backend-app.vercel.app/register
- Body : raw/json

#### Body Example:
{
    "email":"anemail@proton.me",
    "password":"budgify2"
}

#### Result :
{
    "message": "User Created Successfully",
    "result": {
        "email": "anemail@proton.me",
        "password": "$2b$10$9Lz3bHM1Z9qqXeoIREUnOe6HcKV8RYueOkm4KFu1Pm8RUefd2sMI.",
        "_id": "673090429fe33381235e7010",
        "__v": 0
    }
}

### User GET

- Method : GET
- URL : https://budgify-backend-app.vercel.app/user/_id

#### Query Example:
https://budgify-backend-app.vercel.app/user/673090429fe33381235e7010

#### Result :
{
    "message": "User found Successfully",
    "result": {
        "email": "chamibot3@proton.me"
    }
}

### Login

- Method : POST
- URL : https://budgify-backend-app.vercel.app/login
- Body : raw/json

#### Body Example:
{
    "email":"anemail@proton.me",
    "password":"budgify2"
}
