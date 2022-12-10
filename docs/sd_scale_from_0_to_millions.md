# System Design : Scale from zero to Millions of Users

## Intro

Designing a system that supports millions of users is challening, and it is a journey
that requires continious refinement and endless improvement. in this document, we build
a system that supports a single user and gradually scale it up to serve millions of users.

### Single Server Setup

A journey of thousand miles begins with a single step, and building a complex system is no different.
To start with something simple, everything is running on a single server.

#### Figure 1-1 shows Single Server Setup

1. Users access websites through domain names, such as `api.mysite.com`. Usually, the DNS is a paid service
provided by third parties and not hosted by our servers.

2. Internet Protocol (IP) addres is returned to the browser or mobile app. 