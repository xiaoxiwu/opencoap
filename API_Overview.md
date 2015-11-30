# Introduction #


# General Design #

Pass in functions needed for OS calls or make a very simple portability wrapper.

Support a mode with no dynamic memory allocation.


# Server API #

General idea is to create a COAP Server object then add callbacks for each resource it supports. At this point queries can be processed and when a resources is accessed, the callback function will get called to get the current value. If a resource changes, the update function can be called so that any subscriptions to the resource will get appropriate notification messages. Each resource is assigned a unique integer ID.


# Client API #