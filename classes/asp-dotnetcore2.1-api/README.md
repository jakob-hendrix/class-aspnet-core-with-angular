# Class Notes: Building Your First API with ASP.NET Core (2.1)

## HTTP Request Pipeline

Whenever an HTTP/S request comes in, there are 2 parts:

1. the request
2. the response

ASP.NET request pipeline allows us to add middleware that handles the flow of the request, in b oth directions (user -> request -> middleware -> response -> middleware -> user)

## MVC

**MVC** is an architectural pattern. Not the full application architecture. It is used in the **presentaion** layer (Angular is a client-side MVC app).

Consistest of 3 parts:

1. Model: model handles the logic for app data. Can contain code to retrive or store data.
2. View: parts of app that handle the display of data (HTML, Razor, etc)
3. Controller: handles interaction between View and Model (including input). Chooses the model to view to display to the user, and populates with model's data

In an API:

1. Model: still the data
2. View: resource representation (often JSON)
3. Controller: consumer of the API

## Misc

- **wwwroot** is the root directory for handling HTTP requests
- you don't return **data**, you return **resources**
