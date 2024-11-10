# backend-db

## Deployment
- *Backend* : backend-db-rho.vercel.app
- *MongoDB* : mongodb+srv://chamibot:password@cluster0.5dltx.mongodb.net/authDB?retryWrites=true&w=majority&appName=Cluster0

## Endpoints

### Register

- Method : POST
- URL : https://budgify-backend-app.vercel.app/register
- Body : raw/json

#### Body Example:
{
    "email":"anemail@proton.me",
    "password":"codemonk2"
}

### Login

- Method : POST
- URL : https://budgify-backend-app.vercel.app/login
- Body : raw/json

#### Body Example:
{
    "email":"anemail@proton.me",
    "password":"codemonk2"
}
