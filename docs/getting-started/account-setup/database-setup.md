# Database Setup

After creating your project, the only thing left to do is to connect your database. There are two ways to connect your MongoDB Database, one a direct integration with MongoDB Atlas which will empower more features on Cosmocloud, and second is to connect just the database.

## MongoDB Atlas Integration

This is the preferred way to connect to your MongoDB databases. With this integration, Cosmcloud will be automatically be able to connect and integrate with Atlas services.

!!! info "Info"

    This is the preferred way as Cosmocloud will be able to create Search Indexes as well as use other Atlas features directly out of the box.

To connect and integrate your MongoDB Atlas account, follow these steps -

1. [Login](https://account.mongodb.com/account/login) to your MongoDB Atlas account, or create a new account.
2. Create a new MongoDB Atlas cluster, if not already done. You can start with a M0 (Free Forever) cluster and then scale as per need.
3. Visit **Access Manager** tab on your [MongoDB organisation page](https://cloud.mongodb.com/v2#/org).
4. Click on **Create API Key** button on top left. When creating a API Key -

    1. Add a description such as `API Key for Cosmocloud`.
    2. Make sure you add the permission **Organisation Read Only** from the Permissions dropdown, without which the integration would not work.
    3. Copy the generated **Public Key** and **Private Key** that is generated for you. These will not be available to view again, so make sure you have copied them securely.

5. Now visit **Access Manager** again and this time, select your Project Access settings.
   1. Click on the **Invite to Project** and invite the API key user you just created above in your project, giving them **Project Owner** access. This will allow Cosmocloud to integrate perfectly and automatically build connection strings.
6. Come back to Cosmocloud on your project dashboard. Open database configuration via **Application Layer --> Configs**.
7. Make sure you are on **Connect with MongoDB Atlas** tab, as shown below.
8. Fill the required fields -

    - **MongoDB Public Key** - Paste the Public Key you had copied on Step 4.3.
    - **MongoDB Private Key** - Paste the Private Key you had copied on Step 4.3.
    - **MongoDB Project ID** - This is the Project ID of your MongoDB Project, available in Project Settings page.
    - **Cluster Name** - The name of the Database cluster you have spinned up.
    - **Database Name** - The logical name of the database where you want your data stored / already stored.

![Database setup Atlas Integration](/assets/database-setup/db1.png)

## Connecting MongoDB Database Only

Use this way to connect to your MongoDB instance quickly, but this will forbid you to use some features like Full Text Search and Change Data Capture on Cosmocloud. You may also use this feature if you have a self-hosted deployment of MongoDB, by exposing the same to internet and connecting here.

![Database setup Atlas Integration](/assets/database-setup/db2.png)

Fill the required fields as show in screenshot above -
- **MongoDB URI** - The database URI connection string in the format - `mongodb+srv://<username>:<pwd>@<IP_ADDR>`
- **Database Name** - The logical name of the database where you want your data stored / already stored.

!!! info "Info"

    You can also connect to MongoDB Atlas cluster via this method by copy pasting the connection URL.

!!! warning "Warning"

    Make sure you open your database to internet in MongoDB Atlas's Network Access tab by whitelisting 0.0.0.0/0 and opening it to internet.

!!! info "Info"

    Currently, Cosmocloud supports only MongoDB Atlas as the database provider. Further down the line, we would also support more full featured OLTP databases. Reach out to us if you need any help in data migration.