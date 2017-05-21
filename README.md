# backbone-crud-app
This is a CRUD app using Backbone.js. I used local-storage of backbone.
## Run
You can run this project by index.html itself.
## BackboneJS
BackboneJS is a lightweight JavaScript library that allows to develop and structure the client side applications that run in a web browser. It offers MVC framework which abstracts data into models, DOM into views and bind these two using events.

- HTTP Request
The HTTP client sends a HTTP request to a server in the form of a request message where web browsers, search engines, etc., acts like HTTP clients. The user requests for a file such as documents, images, etc., using the HTTP request protocol. In the above diagram, you could see that the HTTP client uses the router to send the client request.

- Router
It is used for routing the client side applications and connects them to actions and events using URL's. It is a URL representation of the application's objects. This URL is changed manually by the user. The URL is used by the backbone so that it can understand what application state to be sent or present to the user.

The router is a mechanism which can copy the URL's to reach the view. The Router is required when web applications provide linkable, bookmarkable, and shareable URL's for important locations in the app.

In the above architecture, the router sending an HTTP request to the View. It is a useful feature when an application needs routing capability.

- View
BackboneJS views are responsible for how and what to display from our application and they don't contain HTML markup for the application. It specifies an idea behind the presentation of the model's data to the user. Views are used to reflect "how your data model looks like".

The view classes do not know anything about the HTML and CSS and each view can be updated independently when the model changes without reloading the whole page. It represents the logical chunk of the UI in the DOM.

As shown in the above architecture, the View represents the user interface which is responsible for displaying the response for the user request done by using the Router.

- Events
Events are the main parts of any application. It binds the user's custom events to an application. They can be mixed into any object and are capable of binding and triggering custom events. You can bind the custom events by using the desired name of your choice.

Typically, events are handled synchronously with their program flow. In the above architecture, you could see when an event occurs, it represents the model's data by using the View.

- Model
It is the heart of the JavaScript application that retrieves and populates the data. Models contain data of an application, logic of the data and represents the basic data object in the framework.

Models represents business entities with some business logic and business validations. They are mainly used for data storage and business logic. Models can be retrieved from and saved to data storage. A Model takes the HTTP request from the Events passed by the View using the Router and synchronizes the data from the database and sends the response back to the client.

- Collection
A Collection is a set of models which binds events, when the model has been modified in the collection. The collection contains a list of models that can be processed in the loop and supports sorting and filtering. When creating a collection, we can define what type of model that collection is going to have along with the instance of properties. Any event triggered on a model will also trigger on the collection in the model.

It also takes the request from the view, bind events and synchronizes the data with the requested data and sends the response back to the HTTP client.

- Data Source
It is the connection set up to a database from a server and contains the information which is requested from the client. 
