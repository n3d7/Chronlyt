# Chronlyt Privacy

Chronlyt is designed to make personal behavioural data useful to you without turning it into a developer dataset.

## Local-first by default

Chronlyt stores your personal data locally on your device.

This may include:

* Tasks and Goals
* Activities and Focus Sessions
* Brain Dump items
* Learning and content records
* Exercise and sleep entries
* Finance entries
* Rules and reviews
* Saved AI reports
* Application settings
* Network Activity history

Core application data is stored locally in SQLite. Logs, exports and backups are also created locally.

## What Chronlyt sends automatically

Chronlyt does **not** automatically upload your behavioural data.

Chronlyt does not include:

* developer analytics or telemetry;
* third-party analytics SDKs;
* automatic crash-report uploads;
* automatic behavioural-data synchronization.

Normal local tracking and productivity features do not require an account or an internet connection.

## Optional network features

Some features use the network only when enabled or requested by the user.

### Updates

Chronlyt may check GitHub Releases for update information when update checking is enabled or manually requested.

Downloading and installing an update requires user action and update packages are cryptographically verified before installation.

### AI Analysis

AI Analysis is optional and disabled unless configured by the user.

Before sending data to an AI provider, you choose what period and categories to include and can review the data that will be submitted.

The request is sent only after explicit user confirmation.

The selected AI provider receives the information contained in that request and processes it according to that provider's own terms and privacy policy.

### Optional account

Chronlyt can be used without an account.

If you choose to create or sign in to an account, Chronlyt may send the information necessary for authentication and device/session management to the Chronlyt account service.

Google or Apple authentication may also communicate with the corresponding identity provider.

Account operations do not include your Tasks, Activities, Focus Sessions, Goals, notes, finance records, reviews or local application database.

An account does not automatically enable behavioural-data synchronization.

## Network Activity

Chronlyt maintains a local Network Activity journal so you can see when supported network operations occur.

The journal may contain information such as:

* operation type;
* destination host;
* status;
* time;
* relevant high-level category information.

It is designed not to record API keys, authentication secrets or submitted payload contents.

## Background Mode and Start at Login

Running Chronlyt in the background or starting it automatically with your operating system does not itself enable additional data collection or network access.

Background operation allows already-enabled local features such as Focus Sessions, Activity Check-ins and notifications to continue while the main window is closed.

It does not automatically start AI Analysis or other optional data-sharing operations.

## Exports and backups

Data Export is generated locally and does not require an AI provider or cloud service.

Backups may contain sensitive personal and behavioural information because they include application data.

Authentication credentials and AI API keys are designed to remain in the operating system's secure credential storage and are excluded from normal exports and backups.

You should protect exported files and backups appropriately, especially when they contain personal information.

## Your control

You can control or disable optional Chronlyt features including:

* Background Mode
* Start at Login
* Activity Check-ins
* automatic update checks
* notifications
* gamification
* AI features

You can also:

* review and clear Network Activity;
* choose which categories to export;
* create local backups;
* remove local Chronlyt data using the application's or operating system's available controls.

## Source code

Chronlyt is a closed-source application.

The public `n3d7/Chronlyt` repository contains product documentation, release information and other public project resources. The application source code is maintained separately and is not published in that repository.
