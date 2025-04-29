## Supervisorctl Commands

Supervisorctl is a command-line tool used to interact with Supervisor, a client/server system that allows its users to monitor and control a number of processes on UNIX-like operating systems. Below are some common commands you may find useful:

### Stop All Processes

### Command

```bash
supervisorctl stop all
```

### Description

This command stops all the processes that are being managed by Supervisor. It is equivalent to issuing a stop command for each individual process.

### Usage

Use this command when you need to stop all processes managed by Supervisor, for example, before performing maintenance or updates.

### Start All Processes

### Command

```bash
supervisorctl start all
```

### Description

This command starts all the processes that are being managed by Supervisor. It is equivalent to issuing a start command for each individual process.

### Usage

Use this command to start all processes managed by Supervisor, typically after maintenance or system updates.

### Additional Resources

For more detailed information on running and managing processes with `supervisorctl`, you can refer to the official documentation: [Supervisor Running Programs](http://supervisord.org/running.html)