> ## 🛠️ Dartvel fork
>
> This is a fork of [`lg-flutter-webos/flutter-webos`](https://github.com/lg-flutter-webos/flutter-webos)
> maintained for the [Dartvel](https://github.com/Danroyal001/dartvel) platform.
> Dartvel drives `dartvel build webos` through this embedder
> (`flutter-webos build webos`), skipping cleanly when it is not installed, and
> `dartvel doctor --target webos` checks that `flutter-webos` is on PATH.
>
> **Why this fork exists:** so Dartvel can pin, patch, and track LG's
> `flutter-webos` embedder against the Flutter version Dartvel ships with.
>
> **Flutter compatibility (verified 2026-07-25):** upstream pins Flutter
> **3.38.10** (revision `c6f67ded`). Dartvel targets **3.44.5**. As with other
> vendor embedders, the webOS engine is a vendor-built artifact, so reaching 3.44
> depends on LG publishing a 3.44 webOS engine; a version-pin bump alone cannot
> work. Native builds and on-device runs require the webOS OSE / TV SDK.
>
> Upstream, docs, and license are unchanged below.

---

# Flutter for webOS

Flutter-webOS is an extension to the Flutter SDK for developing Flutter applications for webOS. 

It provides the necessary tools and libraries to build, package, and run Flutter apps on webOS-powered devices.


## Quick Start 

```
flutter-webos doctor -v
flutter-webos precache -f
flutter-webos devices 

flutter-webos create --platforms webos helloworld
helloworld$ flutter-webos build webos --release
helloworld$ flutter-webos run -d <your_device_id>
```

For detailed installation steps, please refer to the instructions below.

## Required Installations

[Getting Started with Flutter for webOS](./doc/getting-started.md)
- Flutter-webOS CLI
- Flutter-webOS SDK
- webOS NDK

## License
This project is licensed under the [LICENSE](./LICENSE) file.

