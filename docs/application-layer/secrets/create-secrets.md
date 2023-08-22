# Creating Secrets

**Secrets** allows you to store and manage confidential information of our application. You can create `Authentication`,`Database` or `Custom` secrets:

## How to Create a Secret

1. Choose the desired environment from the dropdown menu located at the top right corner for which you wish to
    create secrets.

2. Click on the `Create secret` button in the Secrets section.

3. Give a unique name for the secret you intend to create.

4. Choose the type of secret you want to create: `Authentication`, `Database`, or `Custom`.

5. If you select the `Authentication` secret :

    1. Enable the secret by setting the "Enabled" toggle to true.

    2. Specify the JSON Web Key Set (JWKS) URI, a URL containing public keys for token validation.

    3. Define the intended audience (aud) for the tokens.

    <iframe src="https://drive.google.com/file/d/1FHE1s4Wco5ePoTINzPqgsJpqhWToxwyO/preview" width="720" height="380" allow="autoplay"></iframe>

6. If you select the `Database` option:

    1. Enter name of the database in secret.

    2. Choose the mode for the database secret: Database only or MongoDB Atlas.

    3. If the mode is set to Database:

        1. Provide the required MongoDB URI for connecting to your database.

    4. If the mode is set to MongoDB Atlas:

        1. Enter the projectId, publicKey, privateKey, and clusterName associated with your MongoDB Atlas account.

    5. Review the entered details for accuracy.

    <iframe src="https://drive.google.com/file/d/1S7bz8BuxqL2VyuSd4u_-DFrYYTktYZM6/preview" width="720" height="380" allow="autoplay"></iframe>

7. If you select the `Custom` option:

    1. Enter the key-value pairs as required.

    <iframe src="https://drive.google.com/file/d/1-hSlhRrTnmkTH06prG7MVMpKd4FYoPAk/preview" width="720" height="380" allow="autoplay"></iframe>

8. Click on "Create button" to create the database secret.

9. Integrate the secret into your application's database connection logic.

!!! info "Info"

    `Authentication`, and `Database` secrets can only be created once. For creating multiple secrets select `Custom Secret` instead.
