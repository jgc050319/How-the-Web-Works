## **Part One: Solidify Terminology**

In your own terms, define the following terms:

- What is HTTP?
Hypertext Transfer Protocol or how browsers and servers communicate
- What is a URL?
Uniform Resource Locator or an address
- What is DNS?
Domain Name System (makes URLs and converts them into IP addresses)
- What is a query string?
allows you to payy key-value pairs into the URL
- What are two HTTP verbs and how are they different?
GET (get data from the server) and POST (send data to the server)
- What is an HTTP request?
a request from a client to a server which follows the HTTP protocol
- What is an HTTP response?
a response from a server to a client which follows the HTTP protocol
- What is an HTTP header? Give a couple examples of request and response headers you have seen.
-Headers provide additional information about the request or the response
-Request header:Host, User-Agent, Accept, Cookie, Cache-Control
-Response headers: Content-Type, Last-Modified, Set-Cookie, Cache-Control
- What are the processes that happen when you type “http://somesite.com/some/page.html” into a browser?
This is what it turned into:
https://www6.somesite.com/?template=ARROW_3&tdfs=1&s_token=1693333898.0290930000&uuid=1693333898.0290930000&searchbox=0&showDomain=0&backfill=0 and my computer deemed it not secure and blocked me from seeing it at first.
- Your browser resolves the name into an IP address using DNS
- Your browser makes a request to that IP address, including headers
- The server sends a response
- The browser makes a DOM from that HTML
- The browser makes separate HTTP requests for those resources and receives response from the server for each
## ****Part Two: Practice Tools****

1. Using ***curl***, make a ***GET*** request to the *icanhazdadjoke.com* API to find all jokes involving the word “pirate”
http://www.icanhazdadjoke.com?q=pirate
2. Use ***dig*** to find what the IP address is for *icanhazdadjoke.com*
www.icanhazdadjoke.com. 0       IN      A       172.67.198.173
www.icanhazdadjoke.com. 0       IN      A       104.21.66.15
3. Make a simple web page and serve it using ***python3 -m http.server***. Visit the page in a browser.

## **Part Three: Explore Dev Tools**

Build a very simple HTML form that uses the GET method (it can use the same page URL for the action) when the form is submitted.

Add a field or two to the form and, after submitting it, explore in Chrome Developer tools how you can view the request and response headers.

Edit the page to change the form type to POST, refresh in the browser and re-submit. Do you still see the field in the query string? Explore in Chrome how you can view the request and response headers, as well as the form data.

## **Part Four: Explore the URL API**

At times, it’s useful for your JavaScript to look at the URL of the browser window and change how the script works depending on parts of that (particularly the query string).

[Read about the URL API](https://developer.mozilla.org/en-US/docs/Web/API/URL)

Try some of the code examples in the Chrome Console so that you can get comfortable with the basic methods and properties for instances of the URL class.