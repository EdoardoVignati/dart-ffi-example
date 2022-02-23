# Dart FFI example

Here is a Flutter example with a Dart plugin written in C++

Reference manual: https://docs.flutter.dev/development/platform-integration/c-interop

This is an implementation of the `native_add` function as described in the manual above.

First of all, clone this repository

If you are running on `Xcode` you need must statically link the library as described in Section 2 of the manual

If you are using Android, open this repository in `AndroidStudio` and launch `example/lib/main.dart` on an Android Emulator

The build process of the example app may take a long time.

## Troubleshooting
On Ubuntu:

`fatal error: 'gnu/stubs-32.h' file not found`

Fix:
- `sudo apt-get install g++-multilib libc6-dev-i386`
- `sudo snap remove flutter`
- Install flutter manually : https://docs.flutter.dev/get-started/install/linux