# Node.js Server Crash Bug

This repository demonstrates a bug in a Node.js server where it unexpectedly crashes after handling a certain number of requests.  The provided solution addresses the issue.

## Bug Description

A simple HTTP server is created using Node.js's `http` module. The server responds with a JSON message to each request. However, under load, the server crashes without a clear error message. This is often indicative of a memory leak or unhandled exception within the request handling logic.

## Bug Reproduction

1. Clone this repository.
2. Run `node server.js`.
3. Send multiple requests to `http://localhost:8080` using a tool like `curl` or a load testing application.
4. Observe the server crashing after a certain number of requests. The crash may not be immediate and depends on system resources.

## Solution

The solution involves carefully reviewing the request handling logic to identify and prevent resource leaks or unhandled exceptions.  This can include techniques such as properly closing resources, error handling, and optimizing memory management.  This is a common issue in server-side applications, highlighting the importance of robust error handling and resource management.

## Further investigation

For more advanced debugging, consider using tools such as a debugger, memory profiler (e.g., heapdump), and logging to identify the exact cause of the crash in more complex scenarios.