# QNamedPipe
A portable component that provide local interprocess communication server/client using named pipe

## Summary

QNamedPipe provides simple interprocess communication in local.

Your first running process should be a server
and the second and subsequent processes should be clients.

QNamedPipe automatically creates a thread for the server and waits.
It can receive binary messages from other processes.

Messages are sent unilaterally from the client,
and the server will emit received(bytes) without any reply.

In Microsoft Windows it is implemented with NamedPipe.
On Unix it is implemented by named pipe created on /tmp.

This is a part of [QuickViewer](https://github.com/kanryu/quickviewer).

## License
BSD-2
Copyright (c) 2017, KATO Kanryu
