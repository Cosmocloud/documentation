# Exploring Nodes

## What is a node in flow engine?

Nodes are the fundamental building blocks that power the functionality and versatility of the Flow Engine. These nodes play a pivotal role in shaping the behaviour, logic, and outcomes of your API workflows.
A Node represents an entity that can be connected to other nodes. A node has inputs and outputs, which are the connections between two or more nodes.

The Flow Engine typically comprises seven distinct types of nodes, each serving a specific purpose and collectively enhancing the functionality of your workflow.

- [Conditional Nodes](#conditional-nodes)
- [Database Nodes](#database-nodes)
- [External Nodes](#external-nodes)
- [Loops Nodes](#loops-nodes)
- [Response Nodes](#response-nodes)
- [Storage Nodes](#trigger-nodes)
- [Triggers Nodes](#trigger-nodes)
- [Variables Nodes](#variables-nodes)

## Conditional Nodes

#### If Else

The "If Else" node empowers you to implement conditional logic within your API flow. It enables you to evaluate a condition and perform different actions based on whether the condition is true or false. This node enhances the flexibility of your workflow, allowing you to guide the flow of execution based on specific criteria or outcomes.

#### If Else v2

The "If Else v2" node, offers a streamlined approach to conditional logic in your API flow. Unlike branching into separate flows, it allows you to evaluate a condition and make a choice that leads to the same destination. This simplifies workflow design by converging paths that eventually meet, optimizing the execution of your API flow while maintaining flexibility in decision-making.

#### Switch Case

The "Switch Case" node empowers you to implement multi-way branching logic within your API flow. By utilizing this node, you can evaluate different conditions and direct the flow of execution based on specific cases, enhancing the flexibility and adaptability of your workflow to various scenarios.

## Database Nodes

#### Custom Query Records

The "Custom Query Records" node empowers you to define and execute tailored queries for retrieving records within your API flow, enabling precise data extraction and customization according to your specific requirements.

#### Delete Records

The "Delete Records" node facilitates the removal of specified records from a data source within your API flow, enabling data management and ensuring accurate data maintenance as part of your workflow.

#### Delete Multiple Records

The "Delete Multiple Records" node empowers you to efficiently remove a set of designated records from a data source within your API flow, streamlining data management and enhancing bulk data deletion capabilities in your workflow.

#### Fetch Records

The "Fetch Record" node empowers you to retrieve specific records from a data source within your API flow, facilitating data extraction and integration for further processing or analysis as part of your workflow.

#### Insert Record

The "Insert Record" node empowers you to add new data entries into a data source within your API flow. By utilizing this node, you can seamlessly integrate new information, enhancing data management and expanding your workflow's capabilities.

#### Insert Multiple Records

The "Insert Multiple Records" node allows you to efficiently add multiple new data entries into a data source within your API flow. This streamlines the process of integrating multiple pieces of information, enhancing data management and enabling bulk data insertion as part of your workflow.

#### List Records

The "List Records" node empowers you to retrieve a list of records from a data source within your API flow. By utilizing this node, you can efficiently extract data, facilitating data analysis, processing, and integration as part of your workflow.

#### Update Records

The "Update Records" node enables you to modify existing data entries within a data source within your API flow. By utilizing this node, you can seamlessly integrate updates to specific records, enhancing data management and enabling efficient data maintenance as part of your workflow.

#### Update Multiple Records

The "Update Multiple Records" node empowers you to efficiently modify a set of designated data entries within a data source in your API flow. This node streamlines the process of updating multiple records simultaneously, enhancing data management and optimizing bulk data modification capabilities within your workflow.

## External Nodes

#### API Call

The "API Call" node allows you to easily connect with external APIs within your API flow, enabling smooth interactions and expanding the functionality of your workflow.

## Loops Nodes

#### For Loop

The "For Loop" node empowers you to iterate over a set of values or elements within your API flow, enabling you to perform repetitive actions, apply logic, and process data sequentially as part of your workflow.

#### While Loop

The "While Loop" node empowers you to create a loop within your API flow that continues executing as long as a specified condition is met. By utilizing this node, you can repeatedly perform actions or processes, enhancing automation and enabling dynamic data-driven iterations within your workflow.

## Response Nodes

#### HTTP Response

The "HTTP Response" node allows you to define and send HTTP responses within your API flow, enabling you to communicate outcomes, status codes, and data back to clients or systems interacting with your API. This node is crucial for controlling the behaviour and feedback of your API endpoints.

## Trigger Nodes

#### HTTP Trigger

The "HTTP Trigger" node serves as a starting point for your API flow, enabling external systems to initiate the workflow by sending HTTP requests. This node allows you to define how your API responds when specific HTTP requests are received, facilitating seamless interaction between your API and external applications.

## Variables Nodes

### Arrays

#### Append to Array

The "Append to Array" node facilitates the addition of new elements to an existing array within your API flow, enhancing data manipulation and enabling dynamic array expansion.

#### Contains

The "Contains" node serves to determine whether a specific value is present within a given array, enhancing data analysis and enabling conditional logic within your API flow.

#### Empty Array

The "Empty Array" node allows you to create an empty array within your API flow, providing a starting point for data collection and manipulation, and enabling efficient array-based operations as needed in your workflow.

#### Length of Array

The "Length of Array" node enables you to determine the number of elements within an array within your API flow. This functionality enhances your ability to assess and manage array data, facilitating dynamic data manipulation and informed decision-making within your workflow.

#### Reverse Array

The "Reverse Array" node empowers you to reverse the order of elements within an array within your API flow. This functionality enhances your ability to manipulate array data, enabling you to present data in a different sequence and facilitating dynamic data arrangement within your workflow.

### Mathematical

#### Add Variable

The "Add Variable" node optimizes API flows by enabling summation operations, enhancing computational capabilities, and improving workflow efficiency through calculated variables.

#### Complex Maths Expr

The "Complex Math Expression" node empowers you to perform intricate mathematical calculations seamlessly within your API flow, enabling advanced computations and data transformations.

#### Decrement Variable

The "Decrement Variable" node allows you to decrease the value of a variable within your API flow. By using this node, you can perform subtraction operations on the variable, facilitating dynamic data manipulation and enabling iterative calculations as part of your workflow.

#### Divide Variable

The "Divide Variable" node enables you to perform division operations on a variable within your API flow, facilitating numerical calculations and dynamic data transformations as part of your workflow.

#### Increment Variable

The "Increment Variable" node enables you to increase the value of a variable within your API flow. By utilizing this node, you can conduct addition operations on the variable, supporting dynamic data manipulation and iterative calculations within your workflow.

#### Multiply Variable

The "Multiply Variable" node enables you to perform multiplication operations on a variable within your API flow. By utilizing this node, you can conduct numerical calculations and dynamic data transformations, enhancing your workflow's computational capabilities.

#### Subtract Variable

The "Subtract Variable" node enables you to conduct subtraction operations on a variable within your API flow. By utilizing this node, you can perform numerical calculations and dynamic data transformations, enhancing your workflow's computational capabilities and supporting various data-driven scenarios.

### Strings

#### Append to String

The "Append to String" node empowers you to dynamically extend a string within your API flow, enabling flexible content building and dynamic string concatenation.

#### Concat Strings

The "Concatenate Strings" node enables you to effortlessly combine multiple strings within your API flow, facilitating dynamic text creation and versatile content generation.

#### Set Variable

The "Set Variable" node allows you to define and assign values to variables within your API flow. This node is essential for storing and managing data that can be used throughout the workflow, enhancing data manipulation and enabling dynamic value assignments in your workflow logic.

#### Slice String

The "Slice String" node empowers you to extract a portion of a string within your API flow. By utilizing this node, you can manipulate string data, facilitating dynamic text extraction and enabling precise data manipulation within your workflow.

#### To Lower

The "To Lower" node allows you to convert a string to lowercase within your API flow. By using this node, you can ensure uniformity in text formatting, facilitate data manipulation, and improve consistency in your workflow's textual data.

#### To Upper

The "To Upper" node enables you to convert a string to uppercase within your API flow. By utilizing this node, you can ensure standardized text formatting, enhance data manipulation, and maintain consistent capitalization across your workflow's textual data.

#### Trim String

The "Trim String" node empowers you to remove leading and trailing whitespace from a string within your API flow. By utilizing this node, you can enhance data cleanliness, facilitate accurate data processing, and ensure consistent formatting in your workflow's textual data.

### JSON

#### Merge JSON

The "Merge JSON" node allows you to combine and unify multiple JSON objects within your API flow. By using this node, you can seamlessly integrate data from various sources, enhancing data consolidation and enabling comprehensive JSON manipulation as part of your workflow.

#### Build JSON Object

The "Build JSON Object" node allows you to construct and customize JSON data structures effortlessly within your API flow, enhancing data formatting and facilitating seamless integration with other systems.
