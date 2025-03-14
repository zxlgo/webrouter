# WebRouter

WebRouter is a lightweight web router for Zx that provides a simple and efficient way to handle HTTP requests.

### Installation

To install WebRouter, you can use the following command:

```
zxl get https://github.com/zxlgo/webrouter@latest
```

### Usage

Simply include the WebRouter module in your Zx application:

```zxl
use server;
// use webrouter
use zxlgo:webrouter;

// create a new router instance
const router = webrouter.Router(server.request);

// define a route handler
fn handleIndex(request) {
  server.write("Index Route");
}

// register the route handler
router.get("/", handleIndex);

// handle the request
router.handle();
```
