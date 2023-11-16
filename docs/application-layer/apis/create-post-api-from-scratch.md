# Creating a POST request API from Scratch

- Let's consider the task of building a `POST` API to add student data.
- To achieve this, we need to construct a **Database Model**, which will define the schema to store student data in the database.
- Additionally, we must design a **Request Body Model**, responsible for specifying the data structure sent within the `POST` request body of the API.

## Crafting the Database Model
- Suppose we need to store student information such as `name`, `rollNumber`, and `address`, where the `address` comprises `city` and `state` attributes.
- Hence, the database model for this purpose would be structured as follows.

<iframe src="https://drive.google.com/file/d/1uBn0qWSZ7EEF6GspuRfN1yFnevrvzpSn/preview" width="720" height="410" allow="autoplay"></iframe>

## Developing the Request Body Model
- Let's assume the desired payload for the post request is as follows.
```js
    {
        name: string,
        rollNumber: number,
        city: string,
        state: string
    }
```
- This payload will be transmitted from the frontend or client utilizing the API.
- To facilitate this, we need to create a new model of type `Request Body`, describing the expected payload structure.

<iframe src="https://drive.google.com/file/d/1X6qq0h8OM4LpQIZGmxPNaksscZV365Ea/preview" width="720" height="410" allow="autoplay"></iframe>

## Constructing the API
- To begin creating the API, navigate to the APIs section within the application layer on the project dashboard's sidebar.
- If this is your initial API creation, a page will prompt you with a "New API" button.
- Alternatively, if APIs are already some apis created, the listing page will appear, featuring a "Create API" button at the top.
- Clicking the "Create API" button will initiate a pop-up to choose between using create the api using **templates** or **starting from scratch**.
- Opt for "Create from Scratch" and proceed by clicking the "Next" button.
- A form will appear on the subsequent page, prompting you to specify the API details.

    ![Create API page](/assets/apis/create-api-form.png) 

- Complete all the fields such as "API name," "Description," "Request method," "Endpoint," "Query model," "Request body," and "Authenticated."
- The "Query model" field presents the query models you have designed. Query model is used generally in `GET` requests to define the query params.
- Similarly, the "Request body" field displays the available request body models.
- After supplying all the details, click the "Create" button to create your API.

## Demonstrative Video: Creating the API

<iframe src="https://drive.google.com/file/d/1XPt0wjE6yHBYCZ5toziWONe0M9NV4OkU/preview" width="720" height="410" allow="autoplay"></iframe>

## Enhancing the API Workflow
- Navigate to the **Flow** section within the API Details page.
- You will encounter an "HTTP Trigger" node encompassing essential request data such as "Request Endpoint," "Request Method," "Query Parameters," "Request Body," and "Authenticated" status.
- Construct the API workflow within the flow engine. For an understanding of the flow engine's mechanics, consult [this guide](TODO Add path here for flow engine docs).
- To exemplify the creation of the API workflow for storing `Student` records, the following video provides a tutorial on utilizing the flow engine.

<iframe src="https://drive.google.com/file/d/1ky79fobIh_i7807Nj1AsWyndcTb0gM5U/preview" width="720" height="410" allow="autoplay"></iframe>

## API Testing
- To facilitate the functionality of your API, you need to establish a connection between your database and CosmoCloud.
- Access the **Application Layer** through the project dashboard's sidebar and navigate to the **Secrets** section.
- Here, add a Database secret by supplying all the required details. Learn how to create a [Database Secret](/application-layer/secrets/create-secrets) here.
- Once the Database secret is successfully updated that signfies that your database has been connected.
- Now, deploy the APIs along with their associated models. After deployment and it's activation, the APIs become operational.
- With your API ready for use, proceed to the API Details page to copy the API endpoint for testing.
- Utilize **Postman** to test the API by sending data in the required payload format to avoid errors.
- Upon successful testing, your data will be inserted and can be verified in your database.

## Demonstrative Video: API Functionality Showcase

<iframe src="https://drive.google.com/file/d/1xXevDNRhXmaP5xxUOo7jHU6Iqfs5TJ8I/preview" width="720" height="410" allow="autoplay"></iframe>

!!! info "Info"

    - Similar to the `POST` request, PUT` and `PATCH` request also expect a Request Body in the API call. Consequently, creating a Request Body model specific to the PUT request is essential.