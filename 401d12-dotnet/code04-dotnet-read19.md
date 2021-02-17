# Code 401 ASP.NET
## Reading 19
##### (All My Notes are attributed/sourced from the Resources directly preceding them.)

<br>
<br>
<br>

### Summary
* When an identity is created, it can be assigned one or more claims
  * The claims are key value pairs that determine what a user can or cannot do
* Authentication and Authorization is determined when a user is created
  * Authentication determines who the user is
  * Authorization determins what the user can do
    * Authorization can be changed over time after the registration of a user
* There are 3 parts to a JWT Token
  * First part is the Header - This determines what Signature will be used
  * Second part is the Payload - This contains the claims
  * Third part is the Signature - This is the encryption
* When using JWT Tokens, there needs to be communication between Producers and Consumers
  * Producers are the service providers while consumers are the users of the service
  * First they need to Share the Secret
  * Second they need to Prepare the Payload
  * Third they need to Get the Token
  * Fourth they need to Identify the Consumer

<br>
<br>

### Resources
* #### __Claims-based authorization in ASP.NET Core__
  * ##### Author:  Microsoft Docs
  * ##### [Article Source](https://docs.microsoft.com/en-us/aspnet/core/security/authorization/claims?view=aspnetcore-2.1)

### Resources
* #### __Introduction to Authentication with ASP.NET Core__
  * ##### Author:  Andrew Lock
  * ##### [Article Source](https://andrewlock.net/introduction-to-authentication-with-asp-net-core/)

### Resources
* #### __Part 2: JWT to authenticate Servers API’s__
  * ##### Author:  Rachit Gulati
  * ##### [Article Source](https://codeburst.io/jwt-to-authenticate-servers-apis-c6e179aa8c4e)

<br>
<br>
<br>

[<-- Back](../README.md)
