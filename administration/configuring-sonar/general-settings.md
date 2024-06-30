# General settings

The first general setting is the update notifier feature. If this option is enabled, Sonar will check for updates when the server is started. Since Sonar contacts the GitHub API, this feature can be disabled by an administrator.

```yaml
check-for-updates: true
```



This general setting in Sonar is the log player addresses feature. If you disable this feature, Sonar will no longer print the IP addresses of players on the console. This only applies to messages produced by Sonar. Any messages produced by the server are unaffected.

```yaml
log-player-addresses: true
```



The last general setting describes how many players are allowed to be online under the same IP address. If you have a server where people are allowed to use many alt accounts, you might want to increase this number. Any player who tries joining when there are already more than the maximum number of players using the same IP address online will be kicked.

```yaml
max-online-per-ip: 3
```
