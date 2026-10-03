<picture>
  <source media="(prefers-color-scheme: dark)" srcset="lockup-on-dark.svg">
  <img alt="Rostrum" src="lockup.svg" height="64">
</picture>

### A stream mix console for Linux, not a patchbay.

Rostrum splits your game, voice chat, mic, music, alerts and desktop audio into named buses.
Each bus goes to your headphones, to the stream, or to both, and OBS gets one clean
**Rostrum Stream Mix** and one **Rostrum Mic** to capture.

<a href="https://github.com/rostrum-audio/rostrum"><img alt="The Rostrum mixer: Headphones and Stream masters, then Mic, Game, Voice, Music, Alerts and Desktop buses with faders, meters and the apps on each bus" src="https://raw.githubusercontent.com/rostrum-audio/rostrum/main/docs/screenshots/mixer.png" width="720"></a>

- **Buses, not cables.** Discord goes to Voice, Spotify to Music, games to Game, all by
  themselves. Drag an app once and it lands on that bus every time.
- **Two mixes from one console.** Headphones, Stream or Both for every bus, plus per-app volume
  and mute, balance and mono headphones.
- **OBS in one click.** Rostrum sets OBS up, mutes sources that would double your audio, and can
  undo it all. LIVE and REC badges follow OBS, with a warning if you go live with your mic muted.
- **Scenes and hotkeys.** Recall every level at once, fade between scenes, push to talk, panic
  mute, auto-ducking, and the `rostrum` command or D-Bus for Stream Deck buttons.
- **Safe by design.** The mix lives in PipeWire, so audio keeps flowing if Rostrum quits. Your
  mic never falls back to another device on stream unless you allow it.
- **Private.** No telemetry and no accounts. Crash reports and update checks only with your
  say-so.

A native Qt 6 and KDE Kirigami app for any current Linux desktop with PipeWire, developed on
KDE Plasma. Free and open source under Apache-2.0.

**Status:** version 0.1.0. It installs from source on Ubuntu 26.04, Fedora 43 and Arch;
AppImage builds arrive with the first published release.

[**Get Rostrum**](https://github.com/rostrum-audio/rostrum#%EF%B8%8F-installation) ·
[Website](https://getrostrum.dev) · [Wiki](https://github.com/rostrum-audio/rostrum/wiki) ·
[Discussions](https://github.com/rostrum-audio/rostrum/discussions) ·
[Report a bug](https://github.com/rostrum-audio/rostrum/issues)

**Contact:** hello@getrostrum.dev · Security reports: security@getrostrum.dev
