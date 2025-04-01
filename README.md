# cosmic-launcher

**Completely Unresponsive**

## cosmic-panel

https://github.com/user-attachments/assets/ac8dc983-a860-4f48-aba2-94fa28088eab

Problems - 
1. only `cosmic-applet-power` respects sway drawing area. Rest (cosmic-applet-battery/audio/network/input-sources ..etc) voilate the rules and span across multiple workspaces.
2. sway workspaces are not detected (expected)
3. `cosmic-launcher` is non-responsive
4. assecibility settings (magnifier) do not work (non-responsive)

What Parts Work - 
1. cosmic-panel integration with cosmic-settings (Changing opacity/ changing placement on screen for dock and panel/ adding and removing applets)


## cosmic-store
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


## cosmic-files 
(Works Fine)
To replace `Gnome Files`

![2025-04-01T21:03:53,953071587+05:30](https://github.com/user-attachments/assets/f152ac19-731f-422d-bbd1-6609193dea4a)


## cosmic-editor 
(Works Fine)
Replace gedit
![image](https://github.com/user-attachments/assets/5a93bed5-6b17-403c-8cf2-ba18e427b195)

## cosmic-osd

**Not Responsive**

```
[2025-04-01T12:16:02Z ERROR cosmic_settings_subscriptions::upower::kbdbacklight] Error listening to KbdBacklight: org.freedesktop.DBus.Error.UnknownMethod: Object does not exist at path “/org/freedesktop/UPower/KbdBacklight”

thread 'tokio-runtime-worker' panicked at src/subscriptions/polkit_agent.rs:23:66:
called `Result::unwrap()` on an `Err` value: MethodError(OwnedErrorName("org.freedesktop.PolicyKit1.Error.Failed"), Some("An authentication agent already exists for the given subject"), Msg { type: Error, serial: 802, sender: UniqueName(":1.12"), reply-serial: 31, body: Signature("s"), fds: [] })
note: run with `RUST_BACKTRACE=1` environment variable to display a backtrace
Aborted (core dumped)

```

