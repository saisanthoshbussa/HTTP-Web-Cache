# HTTP Web Cache

This project is an HTTP-based Web Cache that stores recently accessed web pages in memory, following a Least Recently Used (LRU) eviction policy. It supports storing a fixed number of web pages and retrieving content either from the cache or via HTTP GET requests.

## Overview

The HTTP Web Cache implementation features include:

- Caching web pages based on the LRU eviction policy.
- Fetching and storing web page content using HTTP GET requests.
- Cache eviction to maintain the fixed cache size.
- Displaying cached URLs in the order of most to least recently used.

## Usage

### Prerequisites

- C/C++ compiler
- Standard C libraries

### Building and Running

1. Clone the repository:

    ```sh
    git clone https://github.com/your_username/http-web-cache.git
    cd http-web-cache
    ```

2. Compile the source code:

    ```sh
    gcc -o http_web_cache http_web_cache.c
    ```

3. Run the program:

    ```sh
    ./http_web_cache
    ```

### Operations

- Enter the URL to fetch the web page content.
- Type 'exit' to quit the cache application.

## Functionality

### Cache Operations

- `moveToFront`: Moves a cached node to the front based on access.
- `evictLRU`: Evicts the least recently used node when the cache is full.
- `fetchPage`: Retrieves web page content using HTTP GET requests.
- `retrievePage`: Fetches or retrieves a web page from the cache.
- `displayCache`: Displays cached URLs in the most to least recently used order.

## Example Usage

Enter URL or 'exit' to quit:
http://www.example.com/page1
Web Page Content:
...
Cache Contents Most to Least Recently Used:

http://www.example.com/page1
Enter URL or 'exit' to quit:
http://www.example.com/page2
Web Page Content:
...
Cache Contents Most to Least Recently Used:

http://www.example.com/page2
http://www.example.com/page1
