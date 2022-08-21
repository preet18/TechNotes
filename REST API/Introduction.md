[20th AUG 2022]()
## REST
Representative State Transfer
It’s an architectural style. APIs which use this Architectural Style are called REST APIs.
So what’s the architecture of Rest? 
The system which follows below format is called Restful Architecture
1.	Client-Server
2.	Uniform Interface

a.	Identification of Resources
b.	Manipulation of resources through representations
c.	Self-descriptive messages
d.	Hypermedia as the engine of application state(HATEOAS)


3.	Layered System
4.	Cache
5.	Stateless
6.	Code-On-Demand

### 1. Client-Server
A system which has a client and a server
### 2. Uniform Interface
All the interfaces are uniform in nature, which means that clients, servers and network based intermediaries interact is uniform/similar in nature
**a.	Identification of Resources**
Each resource has a unique identifier, i.e URI. For eg: a particular home page, URI like http://www.orielly.com, uniquely identifies the websites root resource.

**b.	Manipulation of resources through representations**
Resource from the webserver could be common, but it could be manipulated at the client side as HTML or JSON or anything as per the required way we could represent/manipulate the resource.

**c.	Self-descriptive messages**
A resource desired state could be represented in request message by client. In the same way the current resource state could be represented in the response message by server. 
Example – Metadata could be represented in the HTTP Headers

**d.	Hypermedia as the engine of application State (HATEOAS)**
A resource’s state representation includes links to related resources.

### 3. Layered System
Proxy/gateways between the client and server. These intermediaries are used to enforce security, response caching and load balancing.
### 4. Cache
Response could be cached at client/server side to reduce the latency and load on the server.
### 5. Stateless
Server treats every request from client as separate form one other. It doesn’t maintain the previous state/request details from the client.
### 6. Code-On-Demand
 Sometimes server may send the response which is a code that need to be executed on the client side to consume it. Browser helps the client to execute java applets, Javascript and Flash.

### HTTP 
Hypertext Transfer Protocol
It’s a message format/language used by computers to communicate over the internet.
