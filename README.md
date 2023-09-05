# Saimon API

## Overview

**SaimonAPI** is a comprehensive and user-friendly API that enables users to seamlessly integrate document analysis and chat functionalities into their applications. With our API, a user can easily register, analyze documents, and engage in dynamic conversations with them.

[Documentation](https://1001epochs.github.io/SaimonAPI-SwaggerDocs/).

## Key Features

- **User Registration**: Streamline user onboarding with our user registration feature. Users can register and preview their profiles effortlessly. Access permissions are automatically adjusted based on the selected subscription tier. This ensures that users enjoy the features and usage limits corresponding to their subscription level.

- **Document Interaction**: Upload documents and engage in interactive conversations with them. Easily analyze and gain insights through features such as text extraction and analysis. Our API also keeps a comprehensive chat history, allowing users to review and reference previous interactions for a complete and immersive user experience.

- **Database Integration**: Seamlessly store document details and user data in a secure and efficient PostgreSQL database, ensuring data integrity and accessibility.

-   **Stripe Integration**: Handle subscription payments seamlessly with Stripe. Payment links are displayed in your frontend application for a user-friendly payment experience.

## Pricing
- **Subscription Tiers**:

  - **Basic**: 
    - Messages: 30
    - Max Documents: 2
    - Price: £10

  - **Premium**:
    - Messages: 100
    - Max Documents: 5
    - Price: £20

  - **Pro**:
    - Messages: 500
    - Max Documents: 10
    - Price: £30

The subscription tiers come with predefined message limits and maximum document allowances. However, you have the flexibility to adjust these limits and pricing through Stripe and API configuration to suit your specific needs.

## Getting Started for Developers

**SaimonAPI** is under active development and is built using FastAPI. It is preconfigured to connect to a PostgreSQL instance upon startup, with PostgreSQL typically running using Docker.

Developers should follow these steps to get started:

1. **Clone the Repository**: Clone the **SaimonAPI** repository from [GitHub Repository Link](https://github.com/1001epochs/).

2. **Install Requirements**: Ensure you have the required dependencies installed. Install them using the following command:

   ```
   pip install -r requirements.txt
	```
3.  **Run PostgreSQL**: Start a PostgreSQL instance using Docker or set up a PostgreSQL database as per your requirements. Modify the database configuration in the API accordingly.
    
4.  **Start the API**: Run the API using the following command:
	   ```
	   uvicorn main:app --reload
	  ```
 3.  This will start the API locally, and it will be accessible at `http://127.0.0.1:8000`.
    
4.  **Explore the API**: Although detailed documentation is still in progress, you can access the API's Swagger documentation to explore available endpoints and interact with the API by visiting `http://127.0.0.1:8000/docs`.
    

Feel free to contribute to the development of **SaimonAPI** and check for updates in the repository as development progresses.
 
## Support

Our dedicated team is available to assist you with any questions or issues you may encounter. Contact us via email or your contact person.

### Known Issues
- [ ] Internal server error - failed response, when auth token is invalid 
- [ ] Sends Entire chat history with request, It is bound to run into rate limit issues. send last 20~30 messages
- [ ] Add reset restriction on event renewed.
- [ ] add page restriction.
