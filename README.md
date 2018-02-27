# QNamedPipe
A portable component that provide local interprocess communication server/client using named pipe

## Summary

QNamedPipe provides simple interprocess communication in local.

Your first running process should be a server,
and the second and subsequent processes should be clients.

QNamedPipe automatically creates a thread for the server and waits.
It can receive binary messages from other processes.

Messages are sent unilaterally from the clients,
and the server will emit received(bytes) without any reply.

In Microsoft Windows it is implemented with NamedPipe() API.
On Unix it is implemented by a named pipe file created on /tmp.

This is a part of [QuickViewer](https://github.com/kanryu/quickviewer).

Details to see https://github.com/kanryu/quickviewer/blob/master/QuickViewer/src/main.cpp


## License
BSD-2
Copyright (c) 2017, KATO Kanryu
