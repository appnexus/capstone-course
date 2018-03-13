# Back-end Systems

This section adpated from Reference 1.

In software engineering, the terms front end and back end refer to the separation of concerns between the presentation layer (front end), and the data access layer (back end) of a piece of software, or the physical infrastructure or hardware. In the client–server model, the client is usually considered the front end and the server is usually considered the back end, even when some presentation work is actually done on the server.

## Difference between front-end and back-end systems
Front-end systems interface with the user via a browser or an application. Some popular web technologies include HTML, CSS, and JavaScript, many frameworks like Bootstrap and Angular, as well as JavaScript libraries like jQuery, and CSS extensions like Sass and LESS.

This section adpated from Reference 2.

Typically, back-end systems run server side, and receive and respond to front-end requests. This can be as simple as a static resource, or something like big data processes or restful API's that interface with data stores before returning the computed result. Some examples for back-end languages include Ruby, PHP, Java, C#, Python etc. with lots of supported frameworks like Django for Python, Spring for Java, NodeJs, Symphony for Php etc.

## APIs and REST

### API
An API is an application programming interface that abstracts the back-end details and executes business logic to represent information to the user in a consistent manner. API's help achieve the following:
* Provide a defined interface for requests and responses to the caller
* Abstract business logic and back-end layer (eg. databases, resources) from the caller. You can change anything without the caller knowing.
* Security in the form of authentication, authorization, and preventing attacks like DOS via mechanisms like throttling.
* Validation layer before requests hit the back-end
* Abstract the front-end user facing interface/model from the data access layer model
* Provide a single, uniform layer/experience to all users of the system with one-time coding in one place
* Provide mechanisms for caching or speed up

Eg. A credit card payment transaction using an API shall ensure validation of credit card details, whether there is enough balance in the account, fraud checks if any, make the request to the backend (say database) and update the transaction and respond with the result in one single operation. The API abstracts database details from the caller of the API which would be impossible to achieve otherwise.

### RESTful API
A RESTful API is an application program interface (API) that uses HTTP requests to GET, PUT, POST and DELETE data. REST stands for "representational state transfer". It is an architectural style and approach to communications often used in web services development. Components of a REST API are:
* URI: Uniform Resource Identifier
* Protocol for communicaton: eg. HTTP
* Data format for exchange: Eg. JSON, XML, protobuf etc.
* Methods: Most common methods include GET, PUT, POST, DELETE with HTTP, other methods exist for CRUD operations.

This section adpated from Reference 3.

REST has gained popularity due to reasons like:
* Much simpler, lightweight, and doesn't require separate client-server programs like SOAP
* HTTP methods are uniform and have clear meaning and distinction
* Performs well, is highly scalable, simple, and easy to modify and extend. This is due to the fact that information produced is separated from technologies that facilitate production and consumption.

Other protocols exist like SOAP (Simple Object Access Protocol) which is more heavy weight but has added security, GraphQL which is a game changer that can solve problems that REST cannot.

## Other examples of backend technologies
* Big data processing in the background applying business logic, mapping and aggregating data into meaningful streams
* Offline ETL's/scripts performing some business function.

Eg. big data streaming or MR jobs that gather information about various auction level impressions in adtech industry and combine them with user events like views and clicks for attribution, offline web scraping and indexing of keywords and attributes for web pages by search engines, ETL's that pull data from various data sources into a data lake or warehouse for reporting and querying etc.

## References
1 [Front and back ends](https://en.wikipedia.org/wiki/Front_and_back_ends)

2 [A Beginner’s Guide to Back-End Development](https://www.upwork.com/hiring/development/a-beginners-guide-to-back-end-development/)

3 [Why REST is So Popular](https://www.serviceobjects.com/resources/articles-whitepapers/why-rest-popular)
