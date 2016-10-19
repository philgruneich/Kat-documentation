# X-Callback-URL
Kat currently supports GET, POST, DELETE and PUT requests. All of these can be executed through `X-Callback-URLs`. A proper Kat request looks a little like this: 
`kat://GET?url=http://thisismyapi.com&header=title,value&header=title2,value2&body=title3,value3`. 
Below you can find a real example of all request types.

## GET request
`kat://GET?url=http://kat.developerpets.com/api/v1/posts/5`

This translates to a normal GET request for the URL http://kat.developerpets.com/api/v1/posts/5.

## POST request
`kat://POST?url=http://kat.developerpets.com/api/v1/posts/new&body=body,Support-for-spaces-would-be-so-nice-and-is-currently-in-development`

This translates to a POST request for the URL http://kat.developerpets.com/api/v1/posts/new. A body parameter will be passed with the title `body` and the value `Support-for-spaces-would-be-so-nice-and-is-currently-in-development`.

## DELETE request

`kat://DELETE?url=http://kat.developerpets.com/api/v1/posts/5`

This translates to a DELETE request for the URL http://kat.developerpets.com/api/v1/posts/5.



--

Please note: I seem to have found a bug where multiple parameters aren't being parsed correctly. A fix for this is underway.
