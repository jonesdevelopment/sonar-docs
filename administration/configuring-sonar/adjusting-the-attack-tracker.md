# Adjusting the attack tracker

{% hint style="warning" %}
Please only edit the attack tracker settings if you really know what you are doing. Any small misconfiguration might lead to unexpected bugs
{% endhint %}

The attack tracker is a constant background check in Sonar that tracks if the server is under attack or not. If Sonar finds the server to be under attack, the configured measures will take place.



The first setting describes the number of new players trying to join the server in one second in order for an attack to be registered. If the number of joins per second exceeds this value, the attack mode is triggered.

```yaml
min-players-for-attack: 8
```



The second setting describes the minimum length of an attack. The attack mode will always be triggered for the given amount of time, regardless of whether the attack is still ongoing or not. This is done to prevent very short attacks triggering the attack mode multiple times a minute.

```yaml
min-attack-duration: 30000
```

> Note: This value represents the time in milliseconds

\
This setting describes the number of times an incident (attack) has to be reported in order to be acknowledged as an actual, real attack. This is done to prevent server lag or many people joining after a server restart from being detected as an attack.

```yaml
min-attack-threshold: 2
```



The last setting describes how much time has to pass between each detected attack.

```yaml
attack-cooldown-delay: 3000
```

> Note: This value represents the time in milliseconds
