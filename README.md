# open-horizon-cheatsheet

This is a set of my personal notes, tips, and shortcuts for the Open Horizon project.

## Logging and Debugging

```
hzn eventlog list
```

```
hzn service log [serviceName]
```

Find a specific service:

`Old School`

```
sudo tail -f /var/log/syslog | grep myhelloworld[[]
```

`New School`

```
sudo docker logs -f $(sudo docker ps -q --filter name=myhelloworld)
```
