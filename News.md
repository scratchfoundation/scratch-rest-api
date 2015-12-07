### GET `/news`

Returns the latest news items from the Scratch's [Tumblr](blogscratch.tumblr.com) account. This route parses each Tumblr post and returns an array of objects suitable for rendering on the Scratch splash page.

#### Request URL
`https://api.scratch.mit.edu/news`

#### Example Request
```bash
curl -X GET "https://api.scratch.mit.edu/news"
```

#### Example Response
```json
[
    {
        "copy": "Create a project to celebrate the 150th Anniversary of Alice in Wonderland for the new Scratch Design Studio!",
        "headline": "New Scratch Design Studio!",
        "id": 133670008323,
        "image": "https://40.media.tumblr.com/1c34c83f9dcaee31422e88bd88de4f00/tumblr_inline_nwuaehA1SR1szpavb_540.png",
        "stamp": "2015-11-21T18:46:35.000Z",
        "url": "https://scratch.mit.edu/studios/1672164/"
    },
    {
        "copy": "We\u2019re launching the first of many upgrades to the Scratch website! Learn more\u2026",
        "headline": "Updates to Scratch Homepage!",
        "id": 131962619508,
        "image": "https://36.media.tumblr.com/b8e8bc37f38a135a0f873a6fe7788701/tumblr_inline_nwuak8hOun1szpavb_540.png",
        "stamp": "2015-09-26T18:12:32.000Z",
        "url": "https://scratch.mit.edu/discuss/topic/163894/"
    },
    {
        "copy": "Want to know what\u2019s happening on Scratch? Check out the latest video update!",
        "headline": "Scratch Video Update: Episode 11",
        "id": 130146748093,
        "image": "https://40.media.tumblr.com/b563e9425dfca8ac53396d997db312ba/tumblr_inline_nwua1f4Chy1szpavb_540.png",
        "stamp": "2015-09-29T18:55:34.000Z",
        "url": "https://scratch.mit.edu/discuss/topic/154790/"
    }
]
```