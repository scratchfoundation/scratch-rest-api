### GET `/users/:id`

Returns basic information about the specified user based on the provided username.

#### Request URL
`https://api.scratch.mit.edu/users/:id`

#### Request Parameters
* **:id** – the username of the user for whom to get information

#### Example Request
```bash
curl -X GET "https://api.scratch.mit.edu/users/mres"
```

#### Example Response
```json
{
    "history": {
        "joined": "2007-03-07T03:50:14.000Z", 
        "login": "2015-11-25T06:16:12.000Z"
    }, 
    "id": 167, 
    "profile": {
        "avatar": "0/0167.png", 
        "bio": "I&#39;m a professor at the MIT Media Lab. But more important: I&#39;m a member of the Scratch Team! \n\nCheck out my TED talk about Scratch: http://bit.ly/mres-ted-talk", 
        "id": 29, 
        "status": "I&#39;m working on new technologies and activities to support the four P&#39;s of creative learning: Projects, Peers, Passion, and Play"
    }, 
    "username": "mres"
}
```