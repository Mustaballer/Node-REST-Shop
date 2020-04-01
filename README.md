# Node REST Shop

This is a Node REST API that acts as a shop service. Users must create an account and be authorized and will then get access to create 
products, update, delete, and fetch data based on products(contains images) and orders. The sign in token works for an hour, and then sign in is required again. In order to use all the features Postman is highly recommended.

## Basic Path requests 

* GET request all products with their info: https://mongo-shop-api.herokuapp.com/products
* GET request one product with a specific id: https://mongo-shop-api.herokuapp.com/products/5e7fed1422ca113690f67d06

## Authorize with POSTMAN

In order to create, update, delete both products and orders(also fetch orders) then you must sign up.
* 1. Change to POST request and the path should be https://mongo-shop-api.herokuapp.com/user/signup
* 2. body should be a raw json and should look like this
*` {
      "email": "Any real email",
      "password": "any password"
   } `
*  3. The will return an access token that will last one hour. This token will be then be used for all requests that need auth. In the headers create a new header called `Authorization` and the value should be `Bearer {Token}`

For more requests and info send an email to mus2003.abdul@gmail.com

## Built With

* [Node.js](https://nodejs.org/en/) - JS runtime environment
* [Express](https://expressjs.com/) - Web Framework for Node.js
* [MongoDB](https://www.mongodb.com/) - NoSQL database
* [Mongoose](https://mongoosejs.com/docs/) - ODM library for MongoDB and Node.js
* [Heroku](https://dashboard.heroku.com/apps) - Cloud Service Host

## Authors

* **Mustafa Abdulrahman** - *Primary Creator* - [Mustaballer](https://github.com/Mustaballer)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Huge props to Academind as learning resources
