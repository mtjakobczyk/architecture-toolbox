# APIs

- **Remote Procedure Call (RPC)** APIs are action-oriented (`POST /launchNewJob` + payload)
- **REST APIs** are resource-oriented (`POST /jobs/new` + payload)

## REST
- Both `POST` and `PUT` are used to send data to an API and in this way create or replace resources.
- `POST` requests can be used to launch some operations, especially in the context of `RPC`-styled APIs
- In contrary to `POST`, a `PUT` request is meant to be idempotent. When you call the same PUT request a number of times, it will always produce the same result.
