One of the most critical properties of the REST Architecture (Representational State Transfer) is that it is stateless
and the state gets transferred between the client and the server. I personally always found this to be confusing until
I really learned architecture by actually using it. In this video, I will explain the state transfer in REST by example. 

In a stateful architecture, the client makes a request to the server and the server “remembers” the client. The next
request from the client will be retrieved from the state stored locally in the server. The pros of this are the server
will pick up where they left off with each request, so request throughput is higher in stateful architecture. Another
advantage of the client can send less data through the wire too. The cons of this architecture are if the server is down,
the request cannot be fulfilled and the client is forced to disconnect and reconnect again to another server anyway and
go through the entire process.

However, REST is a stateless architecture where every request is responsible to “bring” as much information about the
client as possible for the server to reconstruct the state from scratch. This mean that no matter what server the client
hit, the request will always be fulfilled so you get higher availability. This is where the state transfer in REST came
from. Disadvantages of this architecture is the client now sends more information through the wire, thus your application
consumes more bandwidth as a result, this is less of an issue with the introduction of protocol buffers and HTTP2. Another
disadvantage is the throughput goes down since each request has to wait for the state to “replay” and get constructed. 
