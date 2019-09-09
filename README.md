## Welcome to the BFIS Integration Issues Repo

## How to use
This repo serves to provide a central place for developers to highlight issues concerning the integration efforts for the BFIS system. Any issues encountered whilst developing middleware to integrate with the provided webservices should be logged as issues in this repo. Developers will respond to issues raised promply and close any issues they feel have been adequately addressed.

### Documentation

Find below the API documentation.

#### Login Endpoint

This endpoint is used to retrieve an access token to use for the other endpoints below. The endpoint requires a username and password which is valid to retrieve an access token as shown below.

**Endpoint:** `https://bfis_host/oauth/token`
**Method:** POST
**Query Parameters:** 
?grant_type=password&username=username&password=password

**Response:**
`
{
   "access_token": "197397c7-a7d2-4360-88ce-39c222381b34",
   "token_type": "bearer",
   "refresh_token": "3f093d3e-f7c2-40e4-9e9e-919e073ee530",
   "expires_in": 3599,
   "scope": "read write trust"
}
`
