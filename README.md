# Specialisation: backend
# 0x00pagination

# Resources
Read or watch:

REST API Design: Pagination HATEOAS Learning Objectives At the end of this project, you are expected to be able to explain to anyone, without the help of Google:

How to paginate a dataset with simple page and page_size parameters How to paginate a dataset with hypermedia metadata How to paginate in a deletion-resilient manner Requirements All your files will be interpreted/compiled on Ubuntu 18.04 LTS using python3 (version 3.7) All your files should end with a new line The first line of all your files should be exactly #!/usr/bin/env python3 A README.md file, at the root of the folder of the project, is mandatory Your code should use the pycodestyle style (version 2.5.*) The length of your files will be tested using wc All your modules should have a documentation (python3 -c 'print(import("my_module").doc)') All your functions should have a documentation (python3 -c 'print(import("my_module").my_function.doc)' A documentation is not a simple word, it’s a real sentence explaining what’s the purpose of the module, class or method (the length of it will be verified) All your functions and coroutines must be type-annotated. Setup: Popular_Baby_Names.csv use this data file for your project 
=====================================================================
# Specialisation: Back-end
0x01-caching
Background Context
In this project, you learn different caching algorithms.

Resources Read or watch:

Cache replacement policies - FIFO
Cache replacement policies - LIFO
Cache replacement policies - LRU
Cache replacement policies - MRU
Cache replacement policies - LFU
Learning Objectives
At the end of this project, you are expected to be able to explain to anyone, without the help of Google:
General:
What a caching system is What FIFO means What LIFO means What LRU means What MRU means What LFU means What the purpose of a caching system What limits a caching system have Requirements Python Scripts All your files will be interpreted/compiled on Ubuntu 18.04 LTS using python3 (version 3.7) All your files should end with a new line The first line of all your files should be exactly #!/usr/bin/env python3 A README.md file, at the root of the folder of the project, is mandatory Your code should use the pycodestyle style (version 2.5) All your files must be executable The length of your files will be tested using wc All your modules should have a documentation (python3 -c 'print(import("my_module").doc)') All your classes should have a documentation (python3 -c 'print(import("my_module").MyClass.doc)') All your functions (inside and outside a class) should have a documentation (python3 -c 'print(import("my_module").my_function.doc)' and python3 -c 'print(import("my_module").MyClass.my_function.doc)') A documentation is not a simple word, it’s a real sentence explaining what’s the purpose of the module, class or method (the length of it will be verified) More Info Parent class BaseCaching All your classes must inherit from BaseCaching defined below:

$ cat base_caching.py #!/usr/bin/python3 """ BaseCaching module """

class BaseCaching(): """ BaseCaching defines: - constants of your caching system - where your data are stored (in a dictionary) """ MAX_ITEMS = 4

def __init__(self):
    """ Initiliaze
    """
    self.cache_data = {}

def print_cache(self):
    """ Print the cache
    """
    print("Current cache:")
    for key in sorted(self.cache_data.keys()):
        print("{}: {}".format(key, self.cache_data.get(key)))

def put(self, key, item):
    """ Add an item in the cache
    """
    raise NotImplementedError("put must be implemented in your cache class")

def get(self, key):
    """ Get an item by key
    """
    raise NotImplementedError("get must be implemented in your cache class")
=============================================================================
# Specialisation: back-end
Resources
Read or watch:
Flask-Babel
Flask i18n tutorial
pytz
Learning Objectives Learn how to parametrize Flask templates to display different languages Learn how to infer the correct locale based on URL parameters, user settings or request headers Learn how to localize timestamps Requirements All your files will be interpreted/compiled on Ubuntu 18.04 LTS using python3 (version 3.7) All your files should end with a new line A README.md file, at the root of the folder of the project, is mandatory Your code should use the pycodestyle style (version 2.5) The first line of all your files should be exactly #!/usr/bin/env python3 All your *.py files should be executable All your modules should have a documentation (python3 -c 'print(import("my_module").doc)') All your classes should have a documentation (python3 -c 'print(import("my_module").MyClass.doc)') All your functions and methods should have a documentation (python3 -c 'print(import("my_module").my_function.doc)' and python3 -c 'print(import("my_module").MyClass.my_function.doc)') A documentation is not a simple word, it’s a real sentence explaining what’s the purpose of the module, class or method (the length of it will be verified) All your functions and coroutines must be type-annotated.
==============================================================================
# Specialisation: backend

# Queuing System in JS

Resources
Read or watch:

Redis quick start
Redis client interface
Redis client for Node JS
Kue deprecated but still use in the industry
Learning Objectives
At the end of this project, you are expected to be able to explain to anyone, without the help of Google:

How to run a Redis server on your machine
How to run simple operations with the Redis client
How to use a Redis client with Node JS for basic operations
How to store hash values in Redis
How to deal with async operations with Redis
How to use Kue as a queue system
How to build a basic Express app interacting with a Redis server
How to the build a basic Express app interacting with a Redis server and queue
Requirements
All of your code will be compiled/interpreted on Ubuntu 18.04, Node 12.x, and Redis 5.0.7
All of your files should end with a new line
A README.md file, at the root of the folder of the project, is mandatory
Your code should use the js extension
Required Files for the Project
package.json
Click to show/hide file contents
.babelrc
Click to show/hide file contents
and…
Don’t forget to run $ npm install when you have the package.json
