# movie-ticket-reservation
Movie ticket reservation system using multithreading

Project description:
Develop a client-server application for ticket reservation system for one day in Cinema halls.
You can use the concept of inter-process communication, multithreading, synchronization,
etc. Supposed you are given H cinema halls. Each cinema halls has N capacity of viewers.
The possible queries made to the system are-
 Inquiry the list of movie.
 Inquiry the number of show and show time for each of the particular movie.
 Inquiry the number of available seat for the particular show.
 Book K ticket for a particular show.
 Cancel a book ticket.

Hint: The master thread creates a list of H cinema halls, and initializes the number of available
seats in each cinema halls to c. Themaster thread then creates S threads that run concurrently in a
loop, and make automatically generated random queriesperiodically. Each query is of one of the
five types mentioned above. During each query (that is, between the beginning and the
(successful) completion of a query), a thread sleeps for arandom short interval (this may, for
example, simulate bank transaction time for booking and cancellation queries). Moreover,
between making two consecutive queries, a thread sleeps for a random short interval. There
should be a limit on number of maximum query can be active at any point to avoid the overload
of the system.
