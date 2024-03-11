# What is MVC?
- It is an architectural pattern.
- Needed to achieve separation of concern.
- MVC stands for Model, View and Controller.
- View represent what the users see (UI/client).
- Views exists on the client side.
- Controller and Model exists on server side.
- Controller collects the incoming requests and passes it to the Model.
- Model contains business logic.
- So, when the model layer computes the results, the controller layer brings it back and send a response to the client.
- Best analogy is, in a restaurant, menu represents the views, waiter represents the controller and chefs represents the model.

## Problems in MVC
- If any of the layer such as contoller or model becomes bulky, the application becomes hard to maintain.
- MVC works for simple small projects but fails for large scale applications.

## Enhanced MVC
* Different layers are follows:
  * Routing layer - Decides who can handle the request. Manages the incoming requests and provide them correct routes.
  * Validation layer - Checks if the incoming request is valid or not. Also validations different inputs such as emails, passwords, etc. This layer won't do anything apart from validation.
  * Controller layer - Forwarding the incoming request to the business logic and decide the response as per the result of the business logic.
  * Service layer - Consists of the core business logic. It never interacts with the DB because DB can change.
  * Repository layer (DAO) - Responsible for DB interaction.
  * Model/Entity layer - Contains the logic to understand how the data is represented in DB. Represents the logical view of schema.
  * Third-party/client/external layer - For third-party api integrations.

### Additional layers
- These layers depends on project to project.
  * View layer - In modern day applications, views are a separate project like a React/Angular/Vue app or any other frontend application.
  * DTO layer - Data transfer object layer.
  * Adapter layer - Design pattern.
  * Config layer - For project's configurations.
  * Constant layer - To store constants.
  * Error layer - To store custom errors.
  * Utils layer - For helper methods.
  * Event layer - For event driven use cases.
  * Test layer - For unit test.