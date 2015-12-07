Welcome to the Scratch REST API! Here you can find information on how to read and write data from and to [Scratch](https://scratch.mit.edu) programmatically. To get started, here's some general information on how our API works, and its current status.

## Getting Started
The Scratch REST API is interactable through HTTPS requests. Though some of our endpoints require that you are an authenticated Scratch user to access, you can easily get started and see how the API works with some of our public enpoints. For example:

`curl -X GET https://api.scratch.mit.edu/users/mres/following`

will return a JSON object containing the list of people user `mres` is following. All API endpoints will fall under the `api.scratch.mit.edu` domain.

## Query Parameters
The API provides two optional query parameters that can be used to limit and/or paginate routes that return an array. `limit` defaults to `20` items which is the maximum number of items that the API will return at any one time. `offset` defaults to `0` but can be any number up to `9007199254740991` (the maximum 64-bit floating point value).

## Rate Limits
coming soon!

## Authentication
coming soon!