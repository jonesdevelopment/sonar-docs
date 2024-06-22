---
description: Brief introduction to Sonar's API and event system
---

# Working with the API

Sonar is supposed to be an easy-to-use plugin; therefore, the API has been designed to give a developer almost full control over the behavior of the plugin.

### Using the API

Before you are actually able to use the API, you will have to add the dependency to your project.&#x20;

```gradle
maven(url = "https://repo.jonesdev.xyz/releases/")
```

{% hint style="danger" %}
Please make sure you do not include the API in your built Jar file by using `compileOnly` instead of `implementation`.
{% endhint %}

```gradle
compileOnly("xyz.jonesdev.sonar:api:<version>")
```

Now you are able to access all the main API functions by using `Sonar.get()`.

### Events

Using Sonar's built-in event system is also not hard. First, you need to create an event listener:

```java
import xyz.jonesdev.sonar.api.event.SonarEvent;
import xyz.jonesdev.sonar.api.event.SonarEventListener;
import xyz.jonesdev.sonar.api.event.impl.UserVerifySuccessEvent;

public final class TestListener implements SonarEventListener {

  @Override
  public void handle(final SonarEvent event) {
    // Check for the event you want to listen for
    // (This is supposed to be a simple API, don't expect annotations, priorities, etc.)
    if (event instanceof UserVerifySuccessEvent) {
      // Cast the event to the event class you previously checked for
      final UserVerifySuccessEvent successEvent = (UserVerifySuccessEvent) event;
      // ...
      System.out.printf("Test: %s (%s) (took %d ms to verify)%n",
        successEvent.getUsername(), successEvent.getOfflineUuid(), successEvent.getTimeTakenToVerify());
      System.out.println("You can also get the raw user data: " + successEvent.getUser());
    }
    // etc.
  }
}
```

Then, you need to register your event listener using the Sonar API:

```java
Sonar.get().getEventManager().registerListener(new TestListener());
```

And - that's it. Have fun developing! If you have any further questions, please feel free to join the [Discord server](https://jonesdev.xyz/discord) and ask in the **#development** chat.
