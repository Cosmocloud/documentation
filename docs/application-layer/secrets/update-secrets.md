# Updating Secrets

Updating your secret is a breeze! Whether it's tweaking settings or changing configurations, you can easily do it all. Here's a step-by-step guide to updating your secret:

## 1. Navigate to the Secret Listing Page

- From the project dashboard, click on the "Secrets" section. You'll see a list of all your secrets you've created.
  
  ![Secrets](/assets/secrets/secret_listing.png)

## 2. Select the Secret to Update

- Find the secret you want to update in the list and click on it. This will take you to the "Secret Details" page of that secret.

## 3. Explore the Editable Sections

- On the "Secret Details" page, you'll see various sections relevant to the selected secret. Some sections will be editable, while others are read-only.

  ![Secrets editable](/assets/secrets/secret_update.png)

## 4. Make Your Changes

- Depending on the secret type, you'll have different editable options. For example:
  - In the "Authentication" secret, you can update `enabled`, `jwksURI` and `Audience` fields.
  - In the "Database" secret, you can update `Mode`, `mongoDB URI`, `projectId`, `Public Key`, `Private Key`, and `Cluster Name` based on the mode selected .
  - In a "Custom" secret, you'll have full flexibility to modify and customize its keys and values.

## 5. Click on Save

- Once you've made the desired changes, click on the "Save" button at the top-right of the page.
- Your changes have been saved, and secret is now updated with the new settings.

  ![Secrets](/assets/secrets/update_confirm.png)
