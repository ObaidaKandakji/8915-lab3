# CST 8915 Lab 3

## Resources

- [Youtube walkthrough](https://youtu.be/Zm-SnyETcas)
- [Product Service Demo](https://github.com/ObaidaKandakji/product-service-demo)  
- [Order Service Demo](https://github.com/ObaidaKandakji/order-service-demo)  
- [Store Front Demo](https://github.com/ObaidaKandakji/store-front-demo)  


---

## Reflection Questions

### i. What challenges did you encounter when configuring environment variables in the GitHub Actions workflow?
One major challenge I faced was that I couldn’t build a Static Web App because of limitations with my student account, so I was forced to create a VM to host the storefront. I also ran into issues with loading products, which turned out to be caused by not adding `https` in front of the updated Vue locations. What confused me most was that the individual tests for the product, service, and order services would not work if I added `https`, but the storefront required it to load correctly. This mismatch led to a lot of trial and error before I figured it out.

### ii. How does deploying microservices on Azure Web App Service differ from running them locally?
Deploying on Azure Web App Service is very differnt from local deployment because the cloud provides both benefits as well as added difficulty. Locally, all the processes happen within an isolated enviornment where configuration as well as debugging is simpler. On Azure, the deployment involves contending with platform limitations, scoping for the application, as well as integration of the application as a whole. It also involves being more mindful of the deployment pipelines as well as resource utilization. In local deployment scenario, this varies less. 

### iii. Why is it important to use environment variables for configurations in a cloud environment?
Using environment variables in a cloud environment is important because they provide a secure and flexible way to manage configuration settings without hardcoding them into the application. They allow the same application code to run across different environments development, testing, and production without modification. This separation improves security by keeping sensitive information like API keys and connection strings out of the source code, and it supports maintainability by making configuration changes easier to manage and update.

