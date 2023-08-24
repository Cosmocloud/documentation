# Create a GET Request API from scratch

- In this section, we'll delve into the process of creating a `GET` API to retrieve student data.
- Our objective is to design an API that retrieves specific student information based on the provided query parameters (if any).

## Designing the Query Model
- To facilitate the retrieval of specific student records, let's start by designing a **Query Params Model** that defines the structure of query parameters.
- Suppose we want to allow querying by `rollNumber` parameter. The `Query Params` model would be as follows:

![Query Params Mode](/assets/apis/query_params_model-1.png)

## Creating the API
- Begin the creation of the `GET` API by navigating to the **APIs** section within the application layer on the project dashboard's sidebar.
- Follow the same steps as before, choosing to "Create from Scratch" if prompted.
- After reaching the API creation form, provide the necessary details including "API name," "Description," "Request method" (set to `GET`), "Endpoint," "Query model," and "Authenticated."
- Select the query model you've designed to enable the use of query parameters.

    ![Create API page](/assets/apis/create-api-form.png) 

- Once all details are provided, proceed by clicking the "Create" button to generate the `GET` API.

## Constructing the API Workflow
- As before, move to the **Flow** section within the API Details page.
- The "HTTP Trigger" node is still relevant, capturing essential request data.
- Construct the API workflow using the flow engine. Reference [this guide](TODO Add path here for flow engine docs) for a comprehensive understanding.
- For our `GET` API, the workflow should encompass retrieving student data based on the specified query parameters.

<!-- Todo add a video here -->

## API Testing
- To assess the functionality of your `GET` API, you can utilize tools such as **Postman** or directly input the API endpoint in a web browser.
- Append the necessary query parameters (e.g., `rollNumber`) to the endpoint URL to retrieve specific student records.

## Demonstrative Video: Creating and Testing the GET API

<!-- Todo add a video here -->

By following these steps, you can successfully create a `GET` API that retrieves student data based on provided query parameters using the designed query model.

!!! info "Info"

    - Similar to the `GET` request, the `DELETE` request can also employ either query parameters or URL parameters to identify the specific data to be deleted.