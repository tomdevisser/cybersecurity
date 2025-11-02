# Processes

Processes are managed by the kernel, each with their own ID known as the _PID_.

Use `ps` to show a list of running processes. To also view processes run by other users and those that don't run from a session (i.e. system processes), run `ps aux`.

`top` gives you real-time statistics on running processes, refreshing every 10 seconds or when browsing using the arrow keys.

`kill <PID>` is used to terminate processes. Some of the possible signals are SIGTERM (allows some cleanup), SIGKILL (doesn't do any cleanup), SIGSTOP (stop/suspend a process).

## Namespaces

The OS uses namespaces to split up the resources (such as CPU, RAM, and priority). They are great for security because it isolates processes from another.

The process with PID 0 is the sustem's init when the system boots, `systemd`. It provides a way of managing processes and sits between the OS and the user. Any program or piece of software that we start is a child process of `systemd`.

`systemctl` allows us to interact with the systemd process/daaemon. E.g. to start Apache, we use `systemctl start apache2`. We can do start, stop, enable and disable.

Processes can run in the foreground and the background (when using `&`). You can also use Ctrl + Z to background a process. Using `fg`, brings a process back to focus.
