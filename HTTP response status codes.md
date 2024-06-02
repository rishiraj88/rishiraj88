# Status Codes for HTTP Response
- PDF file is available here: [PDF](https://github.com/rishiraj88/Status%20Codes%20for%20HTTP%20Response.pdf)
## The following are the five categories of response codes:
- 1xx - informational message
- 2xx - successful message
- 3xx - redirectional message
- 4xx - client error
- 5xx - server error

## 1xx Series
### 100 = Continue
It is an indication to keep the connection active to receive more portions of message body using more requests

## 2xx Series
### 200 = OK
Request was successful and the response body contains the result of the request
### 201 = Created
It is returned in response to a POST request to indicate that a new resource has been created.

## 3xx Series
### 301 = Moved Permanently
It indicates the redirection to a different URL because the requested resource has been relocated ("permanently"). It uses `Location` header. Not to revert to older URL for next requests.
### 302 = Found
It indicates the redirection to a different URL only for the current request. It uses `Location` header. Yes, to revert to older URL for next requests.
### 304 = Not Modified
It instructs web browser to use the cached copy of the requested resource. It uses the headers: `If-Modified-Since` and `If-None-Match`.

## 4xx Series
### 400 = Bad Request
It indicates that client submitted an invalid HTTP request. This response code is used when the server fails to generate `HTTP 404` response.
### 401 Unauthorized
When client tries to access a protected resource without authentication.
### 403 Forbidden
When an authenticated user tries to access a protected resource but the user is not authorized to do so. It indicates that the user lacks the requisite permission on the resource.
### 404 Not Found
When the requested resource does not exist. One frequent scenario for this is malformed URLs.
### 405 Method Not Allowed
When the used HTTP method is not available for use with the requested URL.
### 413 Request Entity Too Large
When the request body is larger than what can be handled by server.
### 414 Request URI Too Long
It indicates that the request URI (URL included) is too large for server to handle.

## 5xx Series
### 500 Internal Server Error
It indicates that there occurred an error in request processing or response preparation such as some error in calculation, string processing or another arithmetic or logical step.
### 503 Service Unavailable
When a server or service is required to assist the main server (or gateway) to process the user request, but the supporting service is not accessible. That service (or service) may be down at all.

## You May Mark your feedback at the Following Contact Points
- **LinkedIn:** <https://www.linkedin.com/in/rishirajopenminds>
- **X:** <https://twitter.com/RishiRajDevOps>
- **Start Page:** <https://bio.link/rishiraj49de>
- **GitHub:** <https://github.com/rishiraj88>

## Credits and Gratitude
I thank all who have mentored, taught and guided me. Also, I appreciate who have supported my work with pair programming and more.
