# Application for close.io

Repository with JSON blob and various ways of submitting it to https://app.close.io/hackwithus/ URI.

# JSON Blob

Create a file called close.io.json and populate with required fields.

```
{
	"first_name": "Sseremba",
	"last_name": "Joseph",
	"email": "jautorun@gmail.com",
	"phone": "+256-701-449-539",
	"cover_letter": "I like React, Redux, Express & MongoDb",
	"urls": [ "https://github.com/jseremba",
	          "https://www.linkedin.com/in/jseremba",
	          "https://twitter.com/jseremba",
	          "https://plus.google.com/+joseph D" ]
}
```

# Posting the Blob
## Using curl

Use curl to post to the URI, make sure that the *--data-binary* argument points to the full path,

```
curl -XPOST -H 'Content-Type:application/json' -H 'Accept: application/json' --data-binary @/home/jseremba/git/close.io/close.io.json https://app.close.io/hackwithus/ -v -s
```
