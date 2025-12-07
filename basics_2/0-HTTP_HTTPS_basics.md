# Basics of HTTP and HTTPS

## 1. Difference between HTTP and HTTPS
**HTTP (Hypertext Transfer Protocol)** is the standard protocol for transferring data over the web. It transmits data in plain text, meaning anyone intercepting the traffic can read it. It typically uses port 80.

**HTTPS (Hypertext Transfer Protocol Secure)** is the secure version of HTTP. It uses SSL/TLS (Secure Sockets Layer / Transport Layer Security) to encrypt the data transferred between the client and the server. This encryption prevents eavesdroppers from reading or tampering with the data. It typically uses port 443.

**Key Difference:** The main difference is **Security**. HTTPS encrypts data, ensuring confidentiality and integrity, while HTTP does not.

## 2. Structure of HTTP Request and Response

### HTTP Request Structure
1.  **Start Line:** Contains the Method (GET, POST), Path (/index.html), and HTTP Version (HTTP/1.1).
2.  **Headers:** Key-value pairs providing metadata (e.g., `Host: google.com`, `User-Agent: Mozilla/5.0`).
3.  **Empty Line:** Separates headers from the body.
4.  **Body (Optional):** Data sent to the server (used in POST/PUT requests).

### HTTP Response Structure
1.  **Status Line:** Contains the HTTP Version, Status Code (200), and Status Message (OK).
2.  **Headers:** Metadata about the response (e.g., `Content-Type: text/html`, `Server: Apache`).
3.  **Empty Line:** Separates headers from the body.
4.  **Body:** The actual content returned (HTML code, JSON data, image bytes, etc.).

## 3. Common HTTP Methods
* **GET**:
    * **Description:** Retrieves data from a server.
    * **Use Case:** Loading a webpage or fetching search results.
* **POST**:
    * **Description:** Submits data to a server to create a new resource.
    * **Use Case:** Submitting a sign-up form or uploading a file.
* **PUT**:
    * **Description:** Updates an existing resource or creates it if it doesn't exist.
    * **Use Case:** Updating a user's profile information completely.
* **DELETE**:
    * **Description:** Removes a specified resource from the server.
    * **Use Case:** Deleting a post or removing a user account.

## 4. Common HTTP Status Codes
* **200 OK**:
    * **Description:** The request was successful.
    * **Scenario:** Standard response for successful HTTP requests (e.g., a page loads correctly).
* **301 Moved Permanently**:
    * **Description:** The URL of the requested resource has been changed permanently.
    * **Scenario:** Redirecting from an old website domain to a new one.
* **403 Forbidden**:
    * **Description:** The client does not have access rights to the content.
    * **Scenario:** Trying to access an admin panel without being logged in as an admin.
* **404 Not Found**:
    * **Description:** The server cannot find the requested resource.
    * **Scenario:** Typing a URL incorrectly or trying to access a deleted page.
* **500 Internal Server Error**:
    * **Description:** The server encountered a situation it doesn't know how to handle.
    * **Scenario:** A bug in the website's code causes the server to crash processing the request.
