# Accounts

An account is optional. Chronlyt's Dashboard, Focus Sessions, Tasks, Activities, reviews, analytics, exports and backups work without signing in.

On first launch choose **Sign in / Create account** or **Continue without account**. You can change this later in **Settings → Account**.

## Sign in methods

- **Google** and **Apple** open your system browser. Chronlyt does not place the provider's login page inside the app.
- **Email and password** requires email verification before the first sign-in.
- **Forgot password?** sends a one-time link. Open it on the computer with Chronlyt, choose a new password, then sign in again.

The account page shows your display name, email, provider and this device. IDs are hidden under Advanced account details.

## Sessions and offline use

Chronlyt restores a valid session after restart using the operating system credential store. If the auth service is offline, your account can show **Offline session** and all local features keep working.

**Sign Out** asks the server to revoke the session and always removes the local stored session. **Remove local session** performs no network request and removes only the credential on this device.

## No sync yet

Creating an account does not upload local data. Cross-device sync, cloud backup and subscriptions are not implemented in this milestone. Data Export remains an independent, offline feature.
