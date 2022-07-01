# Access Token

To make API calls, you will need an access token and a subscription key. 

The access key can be obtained by making an HTTPS POST call to the following URL:

https://fincb2cProduction.b2clogin.com/fincb2cProduction.onmicrosoft.com/oauth2/v2.0/token?p=B2C_1_ROPCPartner&username=[username]&password=[password]&grant_type=password&client_id=e6b4ebd7-eb04-4def-8720-275660831db6&response_type=token id_token&scope=openid e6b4ebd7-eb04-4def-8720-275660831db6 offline_access

Alternatively, you can make a Postman request using our predefined collection.

Pass your login ID [username] and password [password] in the query parameters.

This returns a JSON response with an access_token. Copy this token and paste it somewhere so that it is accessible when you're ready to begin making calls to the API.

# Subscription Key

To obtain your subscription key, use the login ID and password from the email and sign into the FinClusive Development Portal.

Click your name on the top right and select Profile. This is where you'll find your subscription key.

Copy your Primary key and paste it with your access token. You'll need both of these handy when you begin making calls.

# Making an API Call

An API is called by passing the subscription-key has a query parameter and Access token in a header.
