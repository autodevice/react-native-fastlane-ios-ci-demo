# RNFLIOSDemo

A React Native iOS simulator demo app with Fastlane and CI/CD via GitHub Actions.

## Build

```bash
npm install
cd ios && pod install && cd ..
cd ios && bundle install && bundle exec fastlane ios build
```

## CI/CD

The GitHub Actions workflow builds the iOS simulator app using Fastlane and uploads it to AutoDevice on every push to `main`.

### Required Secrets

- `AUTODEVICE_API_KEY` — API key for AutoDevice
