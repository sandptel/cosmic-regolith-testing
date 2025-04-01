## Cosmic Store
**UI Rendering Without Functionality**

- Error
```
Failed to install Foliate from System

Failed to install Foliate (com.github.johnfactotum.Foliate) from 
System (packagekit):
Error while installing package: unable to create '/usr/bin/7z.dpkg-
new' (while processing './usr/bin/7z') (code 58)

```

- Log

```
[<date> WARN  cosmic_store] operation 0 failed: Error while installing package: unable to create '/usr/bin/7z.dpkg-new' (while processing './usr/bin/7z') (code 58)

```
![2025-04-01T17:50:29,538072225+05:30](https://github.com/user-attachments/assets/3f9a0de2-2c54-411d-af81-c18b53938ca0)
![2025-04-01T17:50:18,001267330+05:30](https://github.com/user-attachments/assets/31c45649-22a7-4e06-b860-1345f47e0a24)

## Cosmic Osd 

**Not Responsive**

```
[2025-04-01T12:16:02Z ERROR cosmic_settings_subscriptions::upower::kbdbacklight] Error listening to KbdBacklight: org.freedesktop.DBus.Error.UnknownMethod: Object does not exist at path “/org/freedesktop/UPower/KbdBacklight”

thread 'tokio-runtime-worker' panicked at src/subscriptions/polkit_agent.rs:23:66:
called `Result::unwrap()` on an `Err` value: MethodError(OwnedErrorName("org.freedesktop.PolicyKit1.Error.Failed"), Some("An authentication agent already exists for the given subject"), Msg { type: Error, serial: 802, sender: UniqueName(":1.12"), reply-serial: 31, body: Signature("s"), fds: [] })
note: run with `RUST_BACKTRACE=1` environment variable to display a backtrace
Aborted (core dumped)

```

