# Application to demo Anypoint MQ usage

This application uses a scheduler to generate two different stock quotes. These quotes are send to a queue.
A subscriber is used to get messages from the queue and the header of the message is parsed to identify which application ie. application-1 or application-2 send the message.
if application-1 is detected, the message is sent to a queue for application-1
if application-2 is detected, the message is sent to a queue for application-2

