# HomeOrganizer
WebApp for organisation of shopping lists, own-inflation-calculator,  nutrition, etc.
Moreover this application is supposed to test out best-practises for development with docker + k8s and microservices, CI/CD in general.
Different services should be scalable different

# Use-Cases
- Organising food products
- Organising shopping lists
- Organising recurring shopping lists
- Reminder to go shopping for missing things
- Planning of financials for housekeeping with any number persons with different financial capabilities
- Representation of data cost-development for calculation of private inflation

# Architecture
The application is planned to be setup as microservice. 

## Web-Frontend
- React or Angular
- Authentication by usual Log-In Providers for B2C cases (Sign-In with Google; Sign-In with Microsoft; Sign-In with Facebook)
- Different frontend for different application parts? (e.g. shopping-lists vs data-representation)
- own database for localisation labels?

## Logic-Backend(s)
- Logic-layer for web-frontend and future native app
- each use-case (above are not final) should get their own logic-layer, so it can be scalled differenciated 
- for learning purposes differnt language should be used for creation of backends
  - .NET 7 (latest version)
  - Node.JS
  - Pyhton or R for representation of data 

## Message broker
- Rabbit MQ

## E-Mail reminder Microservice
- Service for sending emails from Message-Quene

# Development
## per Use-Case
1. defining use cases in details (defining duties of application)
2. designing front-end in detail (Adobe XD)
3. creating dev branch for this use-case
4. setting up MVP with 1 use case
