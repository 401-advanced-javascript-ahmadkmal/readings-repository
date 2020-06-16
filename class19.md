# class 19 Message Queues

we do we need massage queue instead of socket , we all know that to send or receive massage from socket we have to stay connected 
but The Queue server is tasked with receiving any published message and then distributing it out to all connected and subscribed clients. It must further ensure that subscribed clients can “catch up” and pull down any messages that they might have missed during a period of disconnection with the server

## Real Time vs Queued Messaging

queue : you will not be scared to lost message
real time : you have to stay connected

