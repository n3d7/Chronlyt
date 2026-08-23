# FAQ

## Does Chronlyt upload my activity?

No. Only optional AI requests send the exact behavioural payload you preview and consent to. Creating an optional account sends identity/device metadata but does not upload Chronlyt history.

## Do I need an AI API or Python?

No. AI is optional, and production packages bundle the analytics sidecar when used.

## Can I use ChatGPT manually?

Yes. Export Markdown/JSON offline and upload it yourself.

## Does core Chronlyt work offline?

Yes. Update checks, optional account operations and explicitly configured AI providers are the only network features. An offline/unavailable account service does not block local use.

## Where is my data stored?

In the operating system's standard per-application data directory resolved by Tauri. **About → Diagnostics** shows the logs path without guessing platform paths.

## Can I back up everything?

Backups cover the local database and metadata. OS-stored AI keys and account session tokens are intentionally excluded and must be configured/restored separately.
