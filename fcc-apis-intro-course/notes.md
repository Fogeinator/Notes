https://www.youtube.com/watch?v=GZvSYJDk-us

# session 1 - intro 👋
Application Programming Interface 🧩
### interfaces
- Anything has an interface, be it buttons / radio / GUI
- Abstracts details and code away from user
- Interfaces evolve overtime, eg Alarm Clock Radios
### developer interfaces 👨‍💻
- like buttons, you don't need to write code that plays music or updates screen when button pressed
- like media player API, you can get music to play
- like web stream API, you can get music from cloud storage 
- you can make anything happen! people have done it for you!
- **note** APIs so widely used, people assume it's Web Based APIs (too useful)
### example 📰
- almost all language got API, eg .toUpper() or .toString()
- devs run into these needs all the time
- they are also deployable
- eg Windows and MACOS filesytem not same, but files open correctly
- so important that there are lawsuits over the language API itself could be copyrighted ***:P***
- all web browsers have APIs that can display webpage correctly, thank god
- frameworks (flask, expressJS, nextJS, reactJS) allows you to route pages
- you need to follow its syntax and follow it tho
- DEVS FIGURE OUT HOW TO USE THESE APIs, the business side

***break***

# session 2 - remote APIs 📺
### importance
- robots, traffic lights, drones, TV remote
- like Shazam, you can never have the whole database on phone - call remote API!
- computational power (google translate camera, very epic and fast)
- there's a lot of history here lol many stuggles but woohoo ***:P***
### REST APIs
Representational State Transfer 
- almost completely took over meaning of APIs
- have limitations, but they are still evolving, eg GraphQL ***:P***
- APIs written in REST still = RESTful API 

***break***

# session 3 - how the web works 🕸
### web structures, hypertext
- browser on computer = client
- connect to server by typing in Universal Resource Locator (URL) or Identifier (URI)
- take http://www.spacejam.com, it has a scheme, HyperText Transfer Protocol
- protocol - a way they communicate (eg I say Hack, you say Club! else the phrase doesnt work)
- browser creates http request with a verb (eg GET when loading, POST when submit form) along with the URI
- server process and responds with HTML body (hypertext markup language)
- http designed as a STATELESS protocol
- if you want state, your client problem dy ***:P***
### request and response 🗣
- you know https://www.youtube.com/watch?v=GZvSYJDk-us see that stuff after (?) that passes info about request
- key and value pairs called "Headers" 
- req and res have headers, saying what they want and give
- popular headers - content-language, content-type, only want page if it changed (powerful caching)
- embed auth in request too, keep logged in across requests
- response headers
- eg Status Code (404, 200 OK), content-type
### REST API constraints and scavenger hunt
- constraints define whether API is RESTful or not
- constraints: 
```
☐ Client-Server Architecture
☐ Statelessness
☐ Layered System
☐ Cacheability
☐ Uniform Design
☐ Code on Demand
```
- how rest sits on top of web technologies:
- client == program, sent request using library probably over Stateless HTTP (server dont know anything about client unless use headers to remember login details)
```
☑ Client-Server Architecture
☑ Statelessness
```
- it was probably requesting a resource (like just about anything) and its collections
- most of the things we want to do to our resources:
` creating, reading, updating, deleting (CRUD)`
- program sends GET req to URI, server responds with data and headers, body typically represented as JSON, the default content-type (Javascript Object Notation)
- HTTP verbs to clarify req in RESTful APIs

| HTTP Verbs | CRUD | 
|---|---|
| GET | Read |
| POST | Create |
| PUT | Update |
| PATCH | Update |
| DELETE | Delete |

- it means any application with RESTAPI means you can pplay with them, and mix and match instances 

***break***

# session 4 - exploring APIs
### spotify for developers
- SDK = software development kit, wraps around API
- read the docs, find https://developer.spotify.com
- web console can test the APIs, get JSON res on browser
- the results are fast because they are cached - nobody can upload new songs every minute lmao
- spotify v powerful, can see recommendeds
- spotify APIcan build epic apps, and other APIs can build cool projects ***:P***
[explored web console]

# session 5 - APIs on CLI
### twilio 
- API company, help devs abstract away communications (whatsapp, calls, texts, telegram)
- example - send txt msg to phone over CLI (but it does cost money tho, legit buy phone number lmao)
[explored web console and CLI POST and GET]

# session 6 - POSTman
