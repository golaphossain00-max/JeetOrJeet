# JEET OR JEET — Android demo starter v1.1

## Added in this version
- Login and registration UI
- Local demo account persistence on the device
- SHA-256 password hash for the local demo credential
- Profile and logout
- Admin panel UI preview
- Bengali/English toggle
- Demo virtual coins and four game tiles

## Build
1. Open this folder in Android Studio.
2. Allow Gradle sync and install Android SDK 35 if requested.
3. Run the `app` configuration on an Android phone or emulator.
4. Create an APK using Build > Build Bundle(s) / APK(s) > Build APK(s).

## Important limitations
This is a local prototype, not a production authentication or admin system. Account data is stored only on the device; there is no backend, OTP, cloud database, real admin authorization, payment gateway, deposits, withdrawals, betting, or cash prizes. SHA-256 here is only a demo credential hash, not a substitute for a production password-hashing service. Do not use real customer credentials.

Any paid features or prize mechanisms must be reviewed against current Indian law and Google Play policy before development. This demo contains no real-money wagering.


## Build APK without a computer
See `PHONE_APK_BUILD_GUIDE_BN.md`. The included GitHub Actions workflow can build a debug APK in the cloud after you upload the project to your own GitHub repository.


## Golden theme update (v1.3)
- Updated the app palette to a black-and-gold premium look.
- Premium membership price target: ₹99/month (display/plan only; no live payment gateway is connected).
- This starter remains a demo: local account storage, virtual coins, and UI-only admin preview. A secure backend, payment provider approval, and production admin authentication are still required.
