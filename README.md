# budget-tracking
Simple PWA budget-tracking app that can be used offline. Access the deployed application [here](https://tranquil-plateau-37868.herokuapp.com/).

## installation
This app uses 3 npm packages [compression](https://www.npmjs.com/package/compression) to compress the backend server code, [mongoose](https://www.npmjs.com/package/mongoose) as the object modeling tool to interact with MongoDB, and the [express](https://www.npmjs.com/package/express) web framework for node.

## usage
This is a simple PWA (progressive web application) that allows a user to track a budget over a period of time. Data is concurrent thanks to MongoDB and IndexedDB. When the user goes offline the pages need for the application to function are cached and the storage switches to indexedDB. This allows the user to access the applicaiton even when they are offline. When they come back online indexedDB will sync with mongoDB for concurrent data no matter the consistency of the users internet.

Each transaction requires a name and an amount. Finally select whether this amount will be a deposit and add to the budget or be a cost and subtract from the budget. 

## screenshots

![image](https://user-images.githubusercontent.com/24512590/74757947-ebbc0900-5233-11ea-9d4e-c1641fb8f600.png)