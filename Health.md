### GET `/health`

Used by the load balancer and related monitoring systems to return the status of a given API node.

#### Request URL
`https://api.scratch.mit.edu/health`

#### Example Request
```bash
curl -X GET "https://api.scratch.mit.edu/health"
```

#### Example Response
```json
{
    "uptime":3083522,
    "load":[
        0.0537109375,
        0.0458984375,
        0.0478515625
    ],
    "sql":{
        "started":"2015-11-24T17:26:38.842Z",
        "min":0,
        "max":20
    }
}
```