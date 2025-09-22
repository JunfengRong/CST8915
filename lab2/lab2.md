
## Video
https://www.youtube.com/watch?v=E18o7ETB6to


## Reflection Questions 

### What changes did you make to the order-service and product-service to comply with the Configurations and Backing Services factors of the 12-Factor App methodology?

•  Independent Repositories – Each service now resides in its own dedicated GitHub repository to ensure clear separation of concerns and independent version control.
•  Order‑Service – The RabbitMQ connection string and the service’s listening port have been externalized to environment variables, removing hard‑coded values from the codebase.
•  Product‑Service – The service’s listening port has been moved to an environment variable, enabling configuration changes without modifying the source code.

### Why is it important to use environment variables instead of hard-coding configurations in your application?



- Separation of Concerns – Storing configuration values in environment variables keeps them separate from the application’s source code. This improves maintainability, as configuration changes can be made without altering or redeploying the codebase.
- Dynamic Updates Without Downtime – Environment variables allow configuration changes to take effect immediately, without requiring a full redeployment. This is especially useful for updating settings in production without interrupting service availability.
- Security and Flexibility – Sensitive information (e.g., API keys, database credentials) can be stored securely outside the code repository, reducing the risk of accidental exposure. It also enables different configurations for development, testing, and production environments without code changes.


### Why is it important to have separate repositories for each microservice? How does this help maintain independence and scalability of each service?

- Independence and Scalability – Each microservice has its own repository, which allows for independent development, testing, and deployment.
- Flexibility and Agility – With separate repositories, it becomes easier to manage and update individual services. 


## Repositories

- Order-service: `https://github.com/JunfengRong/CST8915-lab2-order-service`
- Product-service: `https://github.com/JunfengRong/CST8915-lab2-product-service`
- Store-front: `https://github.com/JunfengRong/CST8915-lab2-store-front`


