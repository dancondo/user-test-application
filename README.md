# User Test Application

This is a repository with the [How-To](#how-to) and [Assumptions](#assumptions) on a simple golang login user API with a react frontend. 

## How-To

   ### Setup Backend
   
   1. Access the [backend](https://github.com/dancondo/user-api) repository, and clone it with
   ```bash
   $ git clone git@github.com:dancondo/user-api.git 
   ```
   2. Follow the readme [How to Run](https://github.com/dancondo/user-api/blob/main/README.md#how-to-run) instructions to get the backend up and running

   ### Setup Front
   
   1. Access the frontend(https://github.com/dancondo/user-api) repository, and clone it with
   ```bash
   $ git clone git@github.com:dancondo/user-api.git 
   ```
   2.  Follow the readme [How to Run](https://github.com/dancondo/user-front/blob/main/README.md#how-to-run) instructions to get the frontend up and running

## Assumptions

   ### Backend
      1. Scoir primary database is MongoDB, so I used it as my database.
      2. While login in, the backend should return an "success message" or "error message", which in my view are better described as an userDto with a jwt token - which may be used for the frontend for further authentication or send an error.
   
   ### Frontend
      1. Scoir uses Mui for its components.
      2. Since the backend reponds with the authentication information in case of success, the frontend is responsible for any message feedback in case of success, otherwise, it will display the errors sent by the backend.
