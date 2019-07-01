# Swoole Server

The structure of the started processes when a server is started in Swoole is described at the [Laravel Swoole](https://github.com/swooletw/laravel-swoole/wiki/2.-Swoole-Structure).

![Swoole Process Structure](https://github.com/AzonMedia/swoole-docs/blob/master/server/swoole_processes_structure.png)

- Master Process: This is the original process when you execute your PHP script. It will fork a main Reactor and a Manager. It is the root process for the whole application.
- Main Reactor: Reactor in Swoole is multi-thread and totally asynchronous implemented with epoll in Linux Kernel or kqueue in OSX. Reactor is in charge of receiving connected requests and deliver to Manager process. In simple words, its function is just like Nginx Server.
- Manager: Manager process will fork multiple Worker processes. When any Worker terminates, it will automatically fork another Worker process to keep an accurate amount of Worker numbers.
- Worker: This is where you should really care about. All the requests(main logics) will be processed in Worker.
- Task Worker: Same function as Worker process, but only for task delivery. Workers can deliver tasks to a task queue asynchronously. And Task Workers are in charge of consuming tasks from this queue.