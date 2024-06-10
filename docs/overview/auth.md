---
# Display h2 to h5 headings
toc_min_heading_level: 4
toc_max_heading_level: 5
---

# Authorization 

The Nmbrs user (ie the Nmbrs customer who you are working with) will need to grant your application permission to access their data via the Nmbrs API. You need to go through the following steps to set up 
authentication with the Nmbrs user.

- **Get your initial authentication credentials**
- [**Get the authorization code**](https://nmbrs.stoplight.io/docs/nmbrs-restapi/e9e0f5292b4a1-authentication#1-get-the-authorization-code)
- [**Exchange the authorization code for the access token**](https://nmbrs.stoplight.io/docs/nmbrs-restapi/e9e0f5292b4a1-authentication#2-exchange-code-for-the-access-token)
- [**Refresh the access token**](https://nmbrs.stoplight.io/docs/nmbrs-restapi/e9e0f5292b4a1-authentication#3-refresh-the-access-token)

## Get your initial authentication credentials

1. If you have not already done so, create account on https://developer.nmbrs.com/ and login
1. Go to ‘My Integrations’, and click the 'ADD APPLICATION' button.
1. Fill in your App name, and your `client_id` will autopopulate.
1. Fill in all other fields and submit.
1. Click on Secrets Tab to get your `client_secret`
1. Subscribe to a product here: https://developer.nmbrs.com/products (Select partner apps - development if you are still developing your app.)

Take note of your `subscription_key`.

The user will grant your app access to their data via an `access_token`. In order to get the `access_token` you must first get a temporary `authorization_code`. 

As the `access_token` needs to be refreshed hourly, you will also need to get a `refresh_token` that will enable you to continue refreshing the `access_token` for 30 days. 

Click on the following links to be taken to the instructions for each task:

- [**Get the authorization code**](https://nmbrs.stoplight.io/docs/nmbrs-restapi/e9e0f5292b4a1-authentication#1-get-the-authorization-code)
- [**Exchange the authorization code for the access token**](https://nmbrs.stoplight.io/docs/nmbrs-restapi/e9e0f5292b4a1-authentication#2-exchange-code-for-the-access-token)
- [**Refresh the access token**](https://nmbrs.stoplight.io/docs/nmbrs-restapi/e9e0f5292b4a1-authentication#3-refresh-the-access-token)

Once you have completed all the above tasks you will be authorized to send CRUD requests to the Nmbrs API.


