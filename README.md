# OpenCart-Fortress & The Complete List of HTTP Status Codes

## Description
This repository contains a variety of `.htaccess` files and configurations, specifically designed to enhance the security of OpenCart installations. These configurations are organized into different folders, with specific `.htaccess` files placed accordingly.

## Prerequisites
Before using the configurations in this repository, please ensure that you have:

1. Apache HTTP Server installed and running.
2. Enabled the `mod_headers` module in your Apache configuration.
3. Sufficient access to place `.htaccess` files within your web server directories.
4. Backed up your existing `.htaccess` files and configurations to prevent any potential loss of data or service disruption.

## Finding Your Server IP Address
You can easily find your server’s IP address by visiting [ipfinder.us](https://ipfinder.us/).

## The Complete List of HTTP Status Codes

HTTP status codes are issued by a server in response to a client's request. They are grouped into five different classes, each representing a range of responses. Below is a comprehensive list of these status codes and their meanings.

## 1XX — Informational
These codes indicate that the server has received the request and the client should continue the request or ignore if it's already finished.

- `100 Continue`: The server has received the headers, and the client should proceed to send the request body.
- `101 Switching Protocols`: The server is switching protocols as requested by the client.
- `102 Processing`: The server has received and is processing the request, but no response is available yet.
- `103 Early Hints`: The server is likely to send a final response with the headers included.

## 2XX — Success
These codes indicate that the client’s request was received, understood, and accepted.

- `200 OK`: Standard response for successful HTTP requests.
- `201 Created`: The request has been fulfilled and resulted in a new resource being created.
- `202 Accepted`: The request has been accepted for processing, but the processing is not complete.
- `203 Non-Authoritative Information`: The server is returning information from a different source.
- `204 No Content`: The server successfully processed the request, but there is no content to send in the response.
- `205 Reset Content`: The server successfully processed the request, and is not returning any content.
- `206 Partial Content`: The server is delivering only part of the resource due to a range header sent by the client.
- `207 Multi-Status`: XML, used to wrap multiple status messages.
- `208 Already Reported`: The members of a DAV binding have already been enumerated in a previous reply to this request, and are not being included again.
- `226 IM Used`: The server has fulfilled a GET request for the resource, and the response is a representation of the result of one or more instance-manipulations applied to the current instance.

## 3XX — Redirection
These codes tell the client that further action needs to be taken in order to complete the request.

- `300 Multiple Choices`: There are multiple options for the resource that the client may follow.
- `301 Moved Permanently`: The requested resource has been assigned a new permanent URI.
- `302 Found`: The requested resource resides temporarily under a different URI.
- `303 See Other`: The response to the request can be found under another URI using a GET method.
- `304 Not Modified`: The resource has not been modified since the last request.
- `307 Temporary Redirect`: The requested resource resides temporarily under a different URI.
- `308 Permanent Redirect`: The requested resource has been permanently moved to a new URI, and any future references should use a new URI with the same semantics.

## 4XX — Client Error
These codes are intended to be used for cases in which the client seems to have made an error.

- `400 Bad Request`: The server cannot or will not process the request due to an apparent client error.
- `401 Unauthorized`: Authentication is required and has failed or has not yet been provided.
- `402 Payment Required`: Reserved for future use.
- `403 Forbidden`: The request was a legal request, but the server is refusing to respond to it.
- `404 Not Found`: The requested resource could not be found but may be available again in the future.
- `405 Method Not Allowed`: A request was made of a resource using a request method not supported by that resource.
- `406 Not Acceptable`: The requested resource is only capable of generating content not acceptable according to the Accept headers sent in the request.
- `407 Proxy Authentication Required`: The client must first authenticate itself with the proxy.
- `408 Request Timeout`: The server timed out waiting for the request.
- `409 Conflict`: The request could not be processed because of conflict in the request, such as an edit conflict.
- `410 Gone`: The resource requested is no longer available and will not be available again.
- `411 Length Required`: The request did not specify the length of its content, which is required by the requested resource.
- `412 Precondition Failed`: The server does not meet one of the preconditions that the requester put on the request.
- `413 Payload Too Large`: The request is larger than the server is willing or able to process.
- `414 URI Too Long`: The URI provided was too long for the server to process.
- `415 Unsupported Media Type`: The request entity has a media type which the server or resource does not support.
- `416 Range Not Satisfiable`: The client has asked for a portion of the file, but the server cannot supply that portion.
- `417 Expectation Failed`: The server cannot meet the requirements of the Expect request-header field.
- `421 Misdirected Request`: The request was directed at a server that is not able to produce a response.
- `422 Unprocessable Entity`: The request was well-formed but was unable to be followed due to semantic errors.
- `423 Locked`: The resource that is being accessed is locked.
- `424 Failed Dependency`: The request failed because it depended on another request and that request failed.
- `425 Too Early`: The server is unwilling to risk processing a request that might be replayed.
- `426 Upgrade Required`: The client should switch to a different protocol.
- `428 Precondition Required`: The origin server requires the request to be conditional.
- `429 Too Many Requests`: The user has sent too many requests in a given amount of time.
- `431 Request Header Fields Too Large`: The server is unwilling to process the request because its header fields are too large.
- `451 Unavailable For Legal Reasons`: The user-agent requested a resource that cannot legally be provided, such as a web page censored by a government.

## 5XX — Server Error
These codes indicate that the server failed to fulfill a valid request.

- `500 Internal Server Error`: A generic error message, given when an unexpected condition was encountered.
- `501 Not Implemented`: The server either does not recognize the request method, or it lacks the ability to fulfill the request.
- `502 Bad Gateway`: The server was acting as a gateway or proxy and received an invalid response from the upstream server.
- `503 Service Unavailable`: The server is currently unavailable (because it is overloaded or down for maintenance).
- `504 Gateway Timeout`: The server was acting as a gateway or proxy and did not receive a timely response from the upstream server.
- `505 HTTP Version Not Supported`: The server does not support the HTTP protocol version that was used in the request.
- `506 Variant Also Negotiates`: Transparent content negotiation for the request results in a circular reference.
- `507 Insufficient Storage`: The server is unable to store the representation needed to complete the request.
- `508 Loop Detected`: The server detected an infinite loop while processing a request.
- `510 Not Extended`: Further extensions to the request are required for the server to fulfill it.
- `511 Network Authentication Required`: The client needs to authenticate to gain network access.

## Disclaimer
The configurations and files provided in this repository are intended to enhance security and are offered "as is" without any warranty of any kind. Neither the authors nor the contributors can be held responsible for any damages or service disruptions that may occur as a result of using or implementing these configurations. It is highly recommended to test these configurations in a secure environment before deploying them to a live server.

## Contributing
Contributions and improvements from the community are always welcome! If you wish to contribute, please follow these steps:

1. Fork the repository.
2. Make your changes or additions.
3. Submit a pull request.

Please ensure that any changes or additions you make maintain the integrity of the security enhancements and adhere to best practices.