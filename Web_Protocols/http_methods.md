# 🌐 HTTP Request Methods

HTTP (Hypertext Transfer Protocol) defines a set of request methods to indicate the desired action to be performed for a given resource.

## Standard Methods:
- **`GET`:** Requests a representation of the specified resource. Safe and idempotent.
- **`POST`:** Submits data to the specified resource, often creating a new entity or causing a state change.
- **`PUT`:** Replaces all current representations of the target resource with the uploaded payload. Idempotent.
- **`PATCH`:** Applies partial modifications to a resource.
- **`DELETE`:** Deletes the specified resource. Idempotent.
- **`HEAD`:** Asks for a response identical to a `GET` request, but without the response body.
- **`OPTIONS`:** Describes the communication options (allowed HTTP methods, CORS headers) for the target resource.
