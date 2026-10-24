# TopNotch

A free macOS menu-bar app that turns the MacBook notch into a live island: what's playing with a live
spectrum and synced lyrics, battery and AirPods glances, weather, your next events, a clipboard history
and a file shelf. This repository only hosts the built app; the source is private.

## Install (Homebrew)

```sh
brew tap vitoudek/tap
brew install --cask vitoudek/tap/topnotch
```

Use the full name `vitoudek/tap/topnotch`. Requires macOS 15 or later.

The first time, right-click TopNotch in Applications and choose **Open** (or System Settings →
Privacy & Security → **Open Anyway**): the app isn't notarized by Apple. Then allow the permissions it
asks for (Bluetooth, Location, Audio capture, Calendars and Reminders), each used only for its feature.

Update: `brew upgrade --cask vitoudek/tap/topnotch` · Remove: `brew uninstall --cask --zap vitoudek/tap/topnotch`

## Privacy

Nothing is collected or sent to the author. Weather sends your location rounded to about 1 km to
[Open-Meteo](https://open-meteo.com); lyrics send the title, artist and album of songs from music apps to
[LRCLib](https://lrclib.net). Calendar, reminders and clipboard data never leave your Mac. Both online
features can be switched off in Settings.

## Terms

TopNotch is free for personal use and provided **as is, without warranty of any kind**. The author is
not liable for any damage or data loss arising from its use. It uses an undocumented macOS feature for
"Now Playing", which a future macOS update may break.
