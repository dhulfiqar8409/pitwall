# Pitwall

Overlays, a voice race engineer and a driving coach for iRacing, in one small Windows program.

- **Overlays**: relative, standings, delta, fuel, inputs, track map with corner numbers, pit helper, lap log, flags, radio transcript and more. Drag them where you want them.
- **Race engineer by voice**: lap times, fuel, flags, cars alongside, pit confirmations. A natural voice with a team-radio sound is included.
- **Coach**: compares every lap with your best, corner by corner, and tells you where the time is.
- **Optional AI**: with your own Anthropic API key, Claude can be your race engineer and answer questions you ask out loud. Everything else works without it.

## Install

1. Open **[Releases](../../releases)** and download **Pitwall-Setup-Full-…exe** (about 900 MB: it includes the voices and speech recognition).
2. Run it. Windows may say "Windows protected your PC" because the program is not signed: choose **More info**, then **Run anyway**.
3. Start iRacing in **borderless** or **windowed** mode (no overlay program can draw over exclusive fullscreen).

No administrator rights are needed. Your laps, track maps and settings are kept in `Documents\Pitwall` and are never touched by Setup or by an uninstall.

## Updates

Pitwall updates itself: it looks here for a newer version and installs it when no sim is running. Nothing to download by hand after the first install.

## First steps

- **Overlays** page: switch overlays on and off, drag them on the miniature. On the sim itself, `Ctrl+Shift+F9` unlocks them for moving and resizing.
- **Coach** page: choose where the engineer's voice plays and which microphone listens. To use Claude, paste your own API key there (it is stored encrypted on your PC).
- **Settings** page: give pit buttons, the talk button and "say again" to buttons on your wheel.

## Privacy

Pitwall runs on your PC. It talks to the internet only for these things:

- to look for updates here;
- to look up a track's official turn numbers the first time you drive it (only the track's name is sent);
- if you add an Anthropic API key, to send your questions and lap data to Claude;
- if you add a Google AI Studio key, to send the sentences the AI engineer speaks to Google, which sends them back as sound.

## Included third-party software

The full Setup also installs these separate programs, unchanged, each under its own licence (see the notice files in the `piper` and `whisper` folders after installing):

- [Piper](https://github.com/rhasspy/piper) text to speech (MIT), with espeak-ng (GPL-3.0-or-later) and ONNX Runtime (MIT)
- Piper voices `en_US-ryan-high` and `en_US-hfc_male-medium` (CC BY-NC-SA 4.0: non-commercial use only)
- [whisper.cpp](https://github.com/ggml-org/whisper.cpp) (MIT) with OpenAI's Whisper large-v3-turbo model (MIT)

## Data from others

Turn numbers and corner names come from [Lovely Track Data](https://github.com/Lovely-Sim-Racing/lovely-track-data), © Lovely Sim Racing, licensed [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/). Pitwall does not include that data: each copy fetches the file for a track when it is first driven and keeps it on that PC.

Pitwall is a hobby project, shared free of charge, with no warranty. It is not affiliated with iRacing.
