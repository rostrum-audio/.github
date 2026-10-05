<picture>
  <source media="(prefers-color-scheme: dark)" srcset="lockup-on-dark.svg">
  <img alt="Rostrum" src="lockup.svg" height="64">
</picture>

### A stream mix console for Linux, not a patchbay.

Rostrum splits your game, voice chat, mic, music, alerts and desktop audio into named buses.
Each bus goes to your headphones, to the stream, or to both. OBS captures
**Rostrum Stream Mix** and **Rostrum Mic** separately.

<a href="https://github.com/rostrum-audio/rostrum"><img alt="The Rostrum mixer: Headphones and Stream masters, then Mic, Game, Voice, Music, Alerts and Desktop buses with faders, meters and the apps on each bus" src="https://raw.githubusercontent.com/rostrum-audio/rostrum/main/docs/screenshots/mixer.png" width="720"></a>

- **Buses, not cables.** Discord goes to Voice, Spotify to Music, games to Game, all by
  themselves. Save its bus with “Always” to keep that placement.
- **Two mixes from one console.** Headphones, Stream or Both for every bus, plus per-app volume
  and mute, balance and mono headphones. Headphones Only excludes Stream Mix sends;
  Stream Only excludes headphone sends.
- **OBS in one click.** Rostrum sets OBS up, mutes sources that would double your audio, and can
  undo applied changes. OBS captures Stream Mix and Rostrum Mic separately; extra app
  or headphone/default-monitor captures can bypass exclusions. Review the preview and make a
  short recording. LIVE and REC badges follow OBS.
- **Check stream readiness.** Inspect controls, devices, channel links and OBS capture
  observations. Verified, Needs attention, Intentionally excluded/idle and Not verified describe
  the evidence. No settings changes, playback or recording; no guaranteed audience audio.
- **Local mic filters.** RNNoise, rumble filter, gate, EQ, compressor and limiter for the stream
  and eligible recording apps, or only the stream, with per-app choices. Audio tools stay plain
  by default. Check Mic plays the Rostrum Mic signal in headphones before OBS.
- **Scenes and hotkeys.** Recall every level at once, fade between scenes, push to talk, panic
  mute, auto-ducking, and the `rostrum` command or D-Bus for Stream Deck buttons.
- **Safe by design.** The mix lives in PipeWire, so audio keeps flowing if Rostrum quits. Your
  saved mic never falls back to another device on stream unless you allow it.
- **Private.** No telemetry and no accounts, and Rostrum does not upload your audio. Crash
  reports are optional. Update checks and automatic AppImage downloads have separate settings;
  OBS communication stays on localhost.

A native Qt 6 and KDE Kirigami app for PipeWire, developed on KDE Plasma.
Free and open source under Apache-2.0.

**Rostrum 0.1.0 is published.** Its x86_64 AppImage was validated in clean Ubuntu 26.04,
glibc 2.43, PipeWire 1.6.2 and WirePlumber 0.5.13, without host Qt/KDE/development packages.
The glibc 2.43 binary floor is not universal Linux compatibility; older glibc and other
architectures are unsupported by this artifact. A working audio session, desktop D-Bus,
X11 or Wayland and host graphics/font libraries are required. Fedora/Arch source-build CI
is separate from AppImage compatibility.

[**Download 0.1.0 AppImage**](https://github.com/rostrum-audio/rostrum/releases/download/v0.1.0/Rostrum-0.1.0-x86_64.AppImage) ·
[SHA256SUMS](https://github.com/rostrum-audio/rostrum/releases/download/v0.1.0/SHA256SUMS) ·
[Release notes](https://github.com/rostrum-audio/rostrum/releases/tag/v0.1.0) ·
[Launch and OBS setup](https://github.com/rostrum-audio/rostrum#appimage-010-x86_64) ·
[Build from source](https://github.com/rostrum-audio/rostrum#build-from-source)

Download the AppImage and SHA256SUMS together, verify with `sha256sum -c SHA256SUMS`,
then `chmod +x Rostrum-0.1.0-x86_64.AppImage` and run it. Without FUSE, use
`./Rostrum-0.1.0-x86_64.AppImage --appimage-extract-and-run`. Fully quit any existing
Rostrum first; builds share settings and a second launch can activate the old instance.

[Website](https://getrostrum.dev) · [Wiki](https://github.com/rostrum-audio/rostrum/wiki) ·
[Discussions](https://github.com/rostrum-audio/rostrum/discussions) ·
[Report a bug](https://github.com/rostrum-audio/rostrum/issues)

**Contact:** hello@getrostrum.dev · Security reports: security@getrostrum.dev
