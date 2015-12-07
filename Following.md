### GET `/users/:id/following`

Returns an array of users that the specified user is following.

#### Request URL
`https://api.scratch.mit.edu/users/:id/following`

#### Request Parameters
* **:id** – the username of the user for whom to get the following list

#### Example Request
```bash
curl -X GET "https://api.scratch.mit.edu/users/mres/following"
curl -X GET "https://api.scratch.mit.edu/users/mres/following?limit=2"
```

#### Example Response
```json
[
    {
        "id":4373272,
        "username":"FunKitten2006",
        "history":{
            "joined":"2014-06-22T22:52:19.000Z",
            "login":"2015-12-04T15:50:56.000Z"
        },
        "profile":{
            "id":4373272,
            "avatar":"437/3272.png",
            "status":"I am working on making Scratch videos to help Scratchers. I now have a new studio called \nTutor Help Studio. I hope this will help a lot of kids on Scratch. Thank you Scratch Team and thanks  too you.","bio":"I love creating stuff on Scratch."
        }
    },
    {
        "id":11756170,
        "username":"cartoonnetwork",
        "history":{
            "joined":"2015-09-09T18:30:33.000Z",
            "login":"2015-12-04T15:27:05.000Z"
        },
        "profile":{
            "id":11756170,
            "avatar":"1175/6170.png",
            "status":"We’re working on our We Bare Bears projects: playing hide and seek with the bears, showing off our sweet b-ball moves, and creating interactive #bearstack stories! Have fun remixing our projects!","bio":"We’re home to a bunch of creative and fun programs like Adventure Time and We Bare Bears, that not only encourage kids to think outside the box, but way outside of their own world."
        }
    }
]
```