## Reflection Questions

### i. What challenges did you encounter when configuring environment variables in the GitHub Actions workflow?
One major challenge I faced was that I couldn’t build a Static Web App because of limitations with my student account, so I was forced to create a VM to host the storefront. I also ran into issues with loading products, which turned out to be caused by not adding `https` in front of the updated Vue locations. What confused me most was that the individual tests for the product, service, and order services would not work if I added `https`, but the storefront required it to load correctly. This mismatch led to a lot of trial and error before I figured it out.

### ii. How does deploying microservices on Azure Web App Service differ from running them locally?
Deploying microservices on Azure Web App Service differs significantly from running them locally because the cloud introduces both advantages and complexities. Locally, everything runs in a controlled environment where debugging and configuration are straightforward. On Azure, deployment requires dealing with platform constraints, scaling options, and service integration. It also requires paying closer attention to deployment pipelines and resource management, which is less of a concern in a local setup. This makes the cloud deployment process more realistic to real-world applications, but also more challenging.

### iii. Why is it important to use environment variables for configurations in a cloud environment?
Using environment variables in a cloud environment is important because they provide a secure and flexible way to manage configuration settings without hardcoding them into the application. They allow the same application code to run across different environments—development, testing, and production—without modification. This separation improves security by keeping sensitive information like API keys and connection strings out of the source code, and it supports maintainability by making configuration changes easier to manage and update.

---

## Resources

- [Product Service Demo](https://github.com/ObaidaKandakji/product-service-demo)  
- [Order Service Demo](https://github.com/ObaidaKandakji/order-service-demo)  
- [Store Front Demo](https://github.com/ObaidaKandakji/store-front-demo)  
- [Project Walkthrough Video](https://youtu.be/Zm-SnyETcas)  
