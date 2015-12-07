### GET `/`

Provides basic information about the API and related support materials. It is intended as a "catch all" for individuals who are exploring or testing the API for the first time.

#### Request URL
`https://api.scratch.mit.edu/`

#### Example Request
```bash
curl -X GET "https://api.scratch.mit.edu/"
```

#### Example Response
```json
{
    "api": "api.scratch.mit.edu",
    "help": "help@scratch.mit.edu",
    "website": "scratch.mit.edu"
}
```