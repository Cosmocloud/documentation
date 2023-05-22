---
sidebar_position: 3
---

# Database setup

Once you have successfully created your project, you would required to set-up your database only the first time. You can do the same in 2 ways -

1. Click on the `Setup your database` item from your Dashboard.
2. Traversing to `Application layer -> Configs` from the left side menu.

> Currently Cosmocloud supports MongoDB Atlas as the database provider. Further down the line, we would also support more full featured OLTP databases. [Reach out to us](https://cosmocloud.io/contact-us) if you need help in Data Migration.

![Databases](/images/db-config.png)

## Connecting your database

- Once on the configuration screen, you would be asked to connect a [MongoDB Atlas](https://www.mongodb.com/atlas) cluster to your project.

- Sign In to your [MongoDB Atlas account](https://account.mongodb.com/account/login), or create a new one in seconds if you don't have one.

- If you are spinning up a new cluster, you can start with a [**Free Forever**](https://www.mongodb.com/docs/atlas/tutorial/deploy-free-tier-cluster/) cluster in MongoDB by selecting an M0 type of cluster. You can then later chose to upgrade as per requirement.

### 1. Configure Network Connectivity

- In order to make Cosmocloud connect to your database successfully, you would have to expose your Database by whitelisting certain IP Addresses.
- To start testing, you can just whitelist `0.0.0.0/0` IP block, which will make any Cosmocloud machine access your DB.
- **[Recommended]** For a better security, you should not open your cluster to `0.0.0.0` (public) but rather [Set Up a Network Peering Connection](https://www.mongodb.com/docs/atlas/security-vpc-peering/). This is allowed for clusters M10 and up. You can [reach out](https://cosmocloud.io/contact-us) to Cosmocloud team for help in connectivity.

### 2. Configure Database Authentication

Once you whitelist IP addresses or setup a network peering connection, you can then add a Database User to your cluster. This would allow only these created users to access your database, even if network is public.

- Create a user named `cosmocloud` with a password of your choice. You can rename your user but this helps in better user management as it is easy to remember.
- Once created, note down the user password securly somewhere, you will require this is the next step.

### 3. Fetch Connection URI

Once you have completed Step 1 and 2, you can then fetch the Database URI following these steps -

- Click the `Connect` button on your Database cluster.
- Chose `Compass` as the access method you will be using. This will easily provide us with the connection URI.
- Chose `I have MongoDB Compass installed` and select the latest version from the dropdown.
- Copy the connection string, which would be similar to - `mongodb+srv://<username>:<password>@<your_cluster>.mongodb.net/`
- Replace `<username>` and `<password>` with the credentials you created in Step 2.
- **Enter this connection string in MongoDB URI section of Cosmocloud's Config section.**
- You can then add the name of your db you want your data to reside in (for ex. `main`).
- Click on **Save**.
