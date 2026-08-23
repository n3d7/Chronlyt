# Background Mode and Start at Login

Chronlyt can keep lightweight desktop functions ready after its main window closes. Both Background Mode and Start at Login are choices: neither is silently enabled.

## First choice

New users see **Keep Chronlyt ready** during onboarding. Existing users see a one-time migration prompt instead of repeating the full onboarding. Choosing **Not now** records the answer and leaves both Background Mode and Start at Login off.

You can change the choices later in **Settings → General → Startup & Background**.

## When the window closes

With **Run in background** enabled, the close button hides the main window. Timestamp-backed Focus Sessions, timer completion, enabled Activity Check-ins, notifications, state persistence, and tray actions remain available. A one-time notice explains that Chronlyt is still running.

With it disabled, the close button quits Chronlyt. The tray's **Quit Chronlyt** action always exits the process, even when Background Mode is enabled. Active Focus state is already stored in SQLite and is recovered from timestamps at the next launch.

The tray provides Open Chronlyt, current Focus status, Start/Show Focus, Pause or Resume, Finish Focus, Brain Dump, Add Activity, and Quit Chronlyt. It refreshes periodically rather than polling every second.

## Start at Login

**Start Chronlyt when I sign in** uses Tauri's operating-system autostart integration on Windows and supported Linux desktop environments. Chronlyt verifies the actual registration after each change; if the operating system rejects it, Settings reports the failure and returns to the real state.

When **Start minimized** is enabled, an autostart launch begins hidden in the tray. A normal manual launch opens the window. If Chronlyt is already running, a second launch activates the existing window instead of opening another SQLite writer.

Linux startup and tray behaviour can vary by desktop environment. A desktop session must provide a compatible system tray/indicator and autostart facility. See [Troubleshooting](troubleshooting.md) for what to include in a privacy-safe bug report.

## Privacy and resources

Background Mode does not enable Activity monitoring, AI, update checks, or any other network feature. Only settings you already enabled continue to operate. The background scheduler runs at a low frequency and does not keep the Python analytics sidecar running.
