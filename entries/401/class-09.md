# WRRC and Java

## HTTP Request Lifecycle 

1. Local processing
  -  Your browser extracts the "scheme"/protocol (we have established
that this will be HTTP), host (www.example.com),
and optional port number, resource path, and query strings that are specified in the form
  - Now that the browser has the intended hostname for the request, it needs to resolve an IP address

2. Like the processing done locally, resolving an IP from a "DNS server"2 is a sequence that includes many steps, and includes failovers if the first request fails to return an address
  - If the cache lookup fails (we will assume it does), your browser fires off a DNS request using UDP
  - Your request will now have to travel many network devices to reach its target DNS server
  - 

3. Establish a TCP Connection
  - client must open a TCP connection
  - One of the key differences between TCP and UDP is that TCP ensures delivery and ordered data transmission
4. Send an HTTP Request
  - The request is made up of a "request line", request header, and a body. The "request line" is simply a line that indicates the HTTP method, the resource being requested, and the protocol version
5. Tearing Down and Cleaning Up
  - Once the response has been fully delivered, the client sends a FIN packet at the TCP level, to which the server responds with an ACK, and then generally sends a FIN of its own


## HTTP request in Java

> built-in Java class HttpUrlConnection

The disadvantages of using this method are that the code can be more **cumbersome** than other HTTP libraries, and it **does not** provide more advanced functionalities such as dedicated methods for adding headers or authentication

`URL url = new URL("http://example.com");`
`HttpURLConnection con = (HttpURLConnection) url.openConnection();`
`con.setRequestMethod("GET");` 

`Map<String, String> parameters = new HashMap<>();`
`parameters.put("param1", "val");`
 
`con.setDoOutput(true);`
`DataOutputStream out = new DataOutputStream(con.getOutputStream());`
`out.writeBytes(ParameterStringBuilder.getParamsString(parameters));`
`out.flush();`
`out.close();`

 
