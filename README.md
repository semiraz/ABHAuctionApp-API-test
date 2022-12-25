# ABHAuctionApp-API-test
Test for testing Auction APIs with Postman and running collections using Newman CLI

## General info

Auction App is a website for auction where users can bid for some product by placing a bid for it. 
A user needs to create an account and log in and then a user can put and sell their product and bid for other products.

## Postman installation
Postman is a lightweight tool the interact with Web Services. 
With Postman you will be able to run this collection.
[Download Postman.](https://www.postman.com/downloads/)

## Newman installation
For Newman installation, first you must be ensure that you have Node.js >= v10. Install [Node.js via package manager.](https://nodejs.org/en/download/package-manager/)
The easiest way to install Newman is using NPM.
For install newman globally on your system, run ```npm install -g newman```

If you want to see nice html report install first ```npm install -g newman-reporter-htmlextra```


## Environment
Homepage: [Auction App](http://ec2-3-67-80-227.eu-central-1.compute.amazonaws.com:8090/ "Auction App")

API Documentation: [Swagger](http://ec2-3-67-80-227.eu-central-1.compute.amazonaws.com:8080/swagger-ui/index.html#/)
## Usage

For using Newman with the Postman API you need to to generate an API key. 
Go to this [link](https://github.com/postmanlabs/newman#using-newman-with-the-postman-api "Generate an API key") to see how to do that.

To run test:

```newman run "https://api.getpostman.com/collections/YOUR_COLLECTION?apikey=YOUR_GENERATED_API_KEY" --environment "https://api.getpostman.com/environments/YOUR_ENVIRONMENT?apikey=YOUR_GENERATED_API_KEY" --reporters=cli,htmlextra```

## Status
This test contains smoke test for Auction App APIs endpoint. 
