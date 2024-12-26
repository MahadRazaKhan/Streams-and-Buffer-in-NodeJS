# Node.js HTTP Server with File Streaming

This repository demonstrates a **Node.js HTTP server** that handles file streaming in three different ways. It showcases how to read and stream data from a file (`input.txt`) to the HTTP response.

![Screenshot](https://miro.medium.com/v2/resize:fit:1134/0*aGm0tL8lJk6CQdKu.png)

---

## Features

- Built using **Node.js** and the **HTTP module**.
- Implements three approaches to handle file streaming:
  - Reading file content with `fs.readFile`.
  - Streaming file content using `fs.createReadStream` with manual chunk handling.
  - Piping the readable stream directly to the HTTP response using `.pipe()`.
- Demonstrates efficient handling of large files.

---

## How It Works

### Three Approaches:
1. **Using `fs.readFile`**: Reads the entire file into memory and sends the content as a response.
2. **Using `fs.createReadStream` (Manual Chunk Handling)**: Streams the file data in chunks, reducing memory usage.
3. **Using `fs.createReadStream` with `.pipe()`**: Simplifies streaming by piping the readable stream directly to the response.

---

![Demo GIF](https://miro.medium.com/v2/resize:fit:1400/1*JfERCAVU1kels69egS3L4A.gif)
