class: middle, center

# Lab 6
### Rest APIs

---

# Contents
- Introduction
- What is an API?
- What is JSON?
- Your Tasks

---

### Lab 6
Display information 
- from the internet
- on your Pi
- using APIs

---

class: middle, center

# APIs
### **A**pplication **P**rogramming **I**nterface

???
- Interface: a way of talking
- Programming: it's for programmers (that's you)!
- Application: lets you make things!

The API lets you call pre-written code.
- e.g. using `GrovePi` Python calls to run the GrovePi code
- e.g. `digitalWrite`

Today, we move to internet APIs
- instead of calling code
- we get information

---

class: middle, center

# REST APIs
### **Re**presentational **S**tate **T**ransfer

???
- state = information
- we want to get the information
  - i.e. transfer it to us

You've already used REST in `mailboxServer.py`
- to send mail to the server
- to get the mail from the server
- these are both transfers

---

# `requests`

```python
import requests

requests.get('http://httpbin.org/get').json()
```

```json
{
  "args": {}, 
  "headers": {
    "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9", 
    "Accept-Encoding": "gzip, deflate", 
    "Accept-Language": "en-US,en;q=0.9", 
    "Dnt": "1", 
    "Host": "httpbin.org", 
    "Upgrade-Insecure-Requests": "1", 
    "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/98.0.4758.80 Safari/537.36", 
    "X-Amzn-Trace-Id": "Root=1-620c6ed9-07b71ba63747d8e305816c3b"
  }, 
  "origin": "207.151.52.238", 
  "url": "http://httpbin.org/get"
}
```

???
To make internet calls, we will use the `requests` library.
As you can see, it's very simple to get started.

Let's talk about the data we received. This is JSON. (Say hello to JSON!)

---

# JSON
### JavaScript Object Notation

```json
{
  "args": {}, 
  "headers": {
    "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9", 
    "Accept-Encoding": "gzip, deflate", 
    "Accept-Language": "en-US,en;q=0.9", 
    "Dnt": "1", 
    "Host": "httpbin.org", 
    "Upgrade-Insecure-Requests": "1", 
    "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/98.0.4758.80 Safari/537.36", 
    "X-Amzn-Trace-Id": "Root=1-620c6ed9-07b71ba63747d8e305816c3b"
  }, 
  "origin": "207.151.52.238", 
  "url": "http://httpbin.org/get"
}
```

???

JSON is a way of representing data, it's ubiquitous on the internet.
uses key-value pairs
- `Dnt` is a key
- 1 is a value
- values can be strings, numbers, arrays, objects, etc.

---

# JSON ❤️ Python

JSON
```json
{
    "name": "John",
    "age": 30,
}
```

Python
```python
import json
print(json.dumps({"name": "John", "age": 30}))

# {"name": "John", "age": 30}
```

???
Python has a built-in JSON library
Python dictionaries are very similar to JSON objects

---

# Your Tasks
1. Get familiar with JSON
2. Make an API call
3. Build an API display with required widgets
4. Make your own widget!

???

So, we've covered 
- what's an API
- what's REST
- what's JSON

---

class: middle, center

# Fin.

???
see if we need to talk about API keys?

Additional popular APIs to demonstrate widespread use:
- https://www.dropbox.com/developers/documentation/http/documentation#check-user
- https://developer.twitter.com/en/docs/twitter-api/tweets/timelines/api-reference