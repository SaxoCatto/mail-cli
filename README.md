# Simple (enough) mail server and client
- File based mail server and client for demonstration sockets and multithreading. Written in C using pthreads.
- SMTP and masochism not on my side for a while :(

## Server
Compile server.c `gcc server.c -lpthread -o server`

Start server by specifying number of threads and listening port `./server [threads] [port]`

## Client
Compile client.c `gcc client.c -lpthread -o client`

Start client by specifiying server's IP and server's listening port `./client [ip] [port]`

# Branches
- Main one kinda broken at time of writing this 'README.md'. A workaround is `-fpermissive`
(or just do a dry run with gcc then patch it)
- `without -fpemissive` is another branch that should be functional in Linux and C17 GCC. Unless I suck
