# Troubleshooting

- **App does not open:** use **About → Open Logs Folder** if available; never attach the database unless you deliberately choose to.
- **Update check failed:** confirm connectivity and GitHub access. Core features remain offline.
- **AI failed:** verify the HTTPS base URL, model and key, then preview again; consent tokens are single-use.
- **Account service unavailable:** keep using local mode and retry later. If a saved account shows Offline session, no local data is blocked or uploaded. A server operator should verify `CHRONLYT_AUTH_BASE_URL`, HTTPS, PostgreSQL and SMTP using the [deployment guide](../authentication.md).
- **Google/Apple sign-in did not return:** close the browser tab and start again. OAuth state is intentionally kept only in memory and expires after ten minutes; restarting Chronlyt invalidates a pending sign-in.
- **Password reset link did not open Chronlyt:** make sure the installed desktop package registered the `chronlyt://` protocol, then request a fresh one-time link. Do not paste the reset URL into a bug report.
- **Linux global shortcut/tray issue:** note distribution, desktop environment and X11/Wayland in a bug report.
- **Start at login could not be enabled:** Chronlyt verifies the operating-system registration and leaves the toggle at the actual state. On Linux, confirm your desktop session supports XDG autostart and try again; do not edit generated startup files while Chronlyt is running.
- **Closing the window did not quit:** Background Mode hides the window by design. Choose **Quit Chronlyt** from the tray, or disable **Settings → General → Startup & Background → Run in background**.
- **Chronlyt started but no window appeared:** an autostart launch may be minimized to the tray. A normal manual launch activates the already-running instance.
- **Sidecar unavailable:** core features continue; packaged releases should include it. Copy privacy-safe diagnostics from About.
