# 🚦 HTTP Response Status Codes

HTTP status codes are issued by a server in response to a client's request made to the server.

## 1. 1xx Informational
- `100 Continue` — Client should continue with its request.
- `101 Switching Protocols` — Server is switching protocols as requested by client (e.g. WebSocket).

## 2. 2xx Success
- `200 OK` — Request succeeded.
- `201 Created` — Request fulfilled and new resource created.
- `204 No Content` — Request succeeded, but returns no body.

## 3. 3xx Redirection
- `301 Moved Permanently` — Target resource assigned a new permanent URI.
- `302 Found` — Temporary redirection.
- `304 Not Modified` — Cached version is still valid.

## 4. 4xx Client Errors
- `400 Bad Request` — Malformed request syntax.
- `401 Unauthorized` — Authentication credentials missing or invalid.
- `403 Forbidden` — Server understands request but refuses authorization.
- `404 Not Found` — Requested resource could not be found.

## 5. 5xx Server Errors
- `500 Internal Server Error` — Generic server crash or error.
- `502 Bad Gateway` — Invalid response received from upstream server.
- `503 Service Unavailable` — Server temporarily overloaded or down for maintenance.
- `504 Gateway Timeout` — Upstream server failed to respond in time.
