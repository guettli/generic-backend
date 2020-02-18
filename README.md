# Generic Backend Vision: No more coding, just config

Request: Client --> Backend --> DB

Response: Client <-- Backend <-- DB

Client: Web-Browser or other http-client.

Backend: A service (Python, Java, Node.js, ...)

DB: Database (PostgreSQL, MongoDB, ...)

# Stone-Age: ..2005

Thin client. The client recevied HTML from the backend.

Custom database and custom backend

No [Object-relational mapping](https://en.wikipedia.org/wiki/Object-relational_mapping) gets used.

# Past: 2005..2015

The client was thin. The client recevied HTML from the backend.

People realized that coding an own/custom database makes no sense. People use PostgreSQL, MySQL, MongoDB, ...

Still lot of backend code.

Most people still use SQL directly. Only few people use ORM.


# Current: 2015..2025

The client is heavy: React or Angular

The backend is simplified. For example [Django REST framework](https://www.django-rest-framework.org/) gets used.


Less backend coding gets done.

ORM gets used almost everywhere

# Future: 2025..

The backend is generic. Like people stopped coding custom databases they stopped coding custom backends.

You define models and permissions and views. But no logic. See [imperative vs declarative](https://www.google.com/search?q=imperative+vs+declarative)

# Conclusion

Generic and well maintained open source tools gain traction. This reduces the custom code size.
