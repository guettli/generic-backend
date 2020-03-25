# Generic Backend Vision: No more coding, just config

Sooner or later the generic backend vision will become reality. No more custom coding in the backend.

No more if-ing and loop-ing. No more [imperative programming](https://en.wikipedia.org/wiki/Imperative_programming) in the backend.

But if you don't need to write "if ... else ..." and "for .. in ... do ..." what do you write?

You will [declare](https://en.wikipedia.org/wiki/Declarative_programming):

* data schema
* permission schema

After the schemas are definied the generic backend will provide you with the interface which is currently en vogue. Either ReST, GraphQL or Protocol-Buffers.

Additional features:

* Automatically created Admin-Interface (like [Django Admin](https://docs.djangoproject.com/en/3.0/ref/contrib/admin/))
* Missing database indexes get detect automatically
* History of changes: You can define which entities/tables should get versioned. 

# History 

I wanted to provide some numbers (years) here. Of course this is not 100% correct, since it is a slow transition from one state to the next.

## "Stone-Age": ..2005

Thin client. The client recevied HTML from the backend.

Custom database and custom backend.

PostgreSQL and MySQL were not wide spread like today. A lot developers time was spent writing
some kind of database or storage engine. Some on top of [Berkeley DB](https://en.wikipedia.org/wiki/Berkeley_DB),
some on top of custom binara data formats stored in files.

No [Object-relational mapping](https://en.wikipedia.org/wiki/Object-relational_mapping) got used.

## Past: 2005..2015

The client was thin. The client recevied HTML from the backend.

People realized that coding an own/custom database makes no sense. People use PostgreSQL, MySQL, MongoDB, ...

Still lot of backend code got done

Most people still use SQL directly. Only few people use ORM.


## Current: 2015..2025

The client is heavy: React or Angular

The backend is simplified. For example [Django REST framework](https://www.django-rest-framework.org/) gets used.

Most developers develop in high level languages. Only very few experts improve the DB core in PostgreSQL, MySQL, ...

Less backend coding gets done.

ORM gets used almost everywhere

Permission handling still gets done in the code with lines like "if user.is_superuser then ... else ..." (Imperative)

Example: The django admin provides a super simple way to get usable interface to edit data in a relational database. But up to now, "Row-Level Security" is not supported by it. I am unsure where it will get implemented: Either in the DB (for example in PostgreSQL) or in the Middleware (for example Django).

## Future: 2025..

The [Bandwagen Effect](https://en.wikipedia.org/wiki/Bandwagon_effect) will choose some winners and some will loose.

If you compare this to version control systems: SVN, bazar, mercurial ... all these alternatives to git have gone. Or like the browser wars. I am so happy, since I don't need a standard and several implementations. One open source implementation (git, Chrome, Linux, ...) is enough.

In 2025 the backend is generic. Like people stopped coding custom databases, they stopped coding custom backends.

You **define** models and permissions and views. But no logic. See [imperative vs declarative](https://www.google.com/search?q=imperative+vs+declarative)

No more imperative permission handling. Set operations (for example SQL) get used to define them.

Related: [Do permission checking via SQL](https://github.com/guettli/programming-guidelines#do-permission-checking-via-sql)

# Next?

You are waiting for source code? From me? Sorry, I won't write this cool generic backend thing.

This is just a README.

If you want it, then code it.
