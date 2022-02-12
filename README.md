# supervisord
supervisord daemon

## USAGE

### CONFIG FILE

(/etc/supervisor/conf.d/process1.conf)
[program:processname]
command=/path/to/p1.bin
autostart=true
autorestart=true
stderr_logfile=/tmp/p2e.log -> error output(2)
stdout_logfile=/tmp/p2o.log -> standart output(1)

## COMMANDS

supervisorctl reread (when config file changed)
supervisorctl update (update)
