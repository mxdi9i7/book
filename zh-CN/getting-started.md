# 1. Getting Started

---

## 1.1 What is web and how does it work?

Any modern website is made up of three important components: Client, Server and Database

### In a Nutshell:

1. Client - The web page that users intereracts with and accepts user input
2. Server - The service that handles the most important business logic on a website
3. Database - The storage of data and information that's generated from a website

### Real world scenario:

#### Client

Take the example of the signup page on facebook.com, the client is the signup page that has a big logo that says Facebook on the left and a signup form that you need to fill out to register. When the user fills out the form and hit the sign up button, the signup form will be sent from the client to the server. This process of sending data to the server is called a **HTTP Request. **Sounds familiar right? Keep reading.

#### Server

The server is basically a program that keeps running on a computer without stopping and waits for requests from the client. When a user signup form is being sent from the client to the server, the server catches that form data and starts processing. The server might need to capitalize your first and last name fields, check if your email address is legit and unique etc. After the server verifies that your signup form passes all the checks that the facebook engineers have setup, your data will be saved into the database. After the data is sent to the database, the server will respond to client and let the client know that the operation was successful. This process of responding to the client after every client request is called the **HTTP Response.** The client will then navigate to a new page if the response says the user is sucessfully created, or display a error message if the user isn't created for any reason.

#### Database

As the new user's signup data enters the database, the user's first name, last name, email address, password etc are then put into their respective _places_ \(we call them columns in SQL and documents in NOSQL\). The database is like a warehouse that stores all the data and information that's generated from your website. You only store what you want to store.

That was a mouthful... here's a cool diagram I drew to help you understand the concept:

The paragraphs on Client, Server and Database basically follows the diagram's flow

## 1.2 Modern problems with the web

Request per second

Imagine the whole process described in the section above happens simultaneously with millions of users at the same time. Wechat for instance had a record signup count of 200,000 per day. The server would need to process millions of data sent to the server















