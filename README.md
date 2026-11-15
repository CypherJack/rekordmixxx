# Rekordmixxx

A Mixxx skin that borrows the look of rekordbox 7's Performance mode. Dark panels, stacked waveforms, blue-line faders, a ringed jog with the BPM in the middle. I wanted the layout I'm used to, running on Mixxx and doing real Mixxx things.

![Rekordmixxx, Dark scheme](skin_preview_Dark.png)

![Rekordmixxx, Amber scheme](skin_preview_Amber.png)

It needs Mixxx 2.4 or newer. It was built and tested on 2.5.6, and this version was also checked on a stock 2.7 development build on macOS. It uses only stock Mixxx widgets, so no patched Mixxx build is needed.

## Install

[**Download the latest release**](../../releases/latest), unzip it, and drop the `Rekordmixxx` folder into your Mixxx skins folder:

| OS | Skins folder |
|---|---|
| Linux | `~/.mixxx/skins/` |
| Linux (Flatpak) | `~/.var/app/org.mixxx.Mixxx/.mixxx/skins/` |
| macOS | `~/Library/Containers/org.mixxx.mixxx/Data/Library/Application Support/Mixxx/skins/` |
| Windows | `%LOCALAPPDATA%\Mixxx\skins\` |

Restart Mixxx, then pick **Rekordmixxx** under Preferences > Interface. There are two colour schemes, Dark (blue) and Amber.

One tip: set Preferences > Waveforms to **Filtered** or **RGB**. The skin colours them like rekordbox's 3-band waveform (blue lows, orange mids, white highs).

## What you get

- A global bar with panel toggles, a clock and master meters
- Stacked waveforms with deck tabs, loop in/out and a zoom strip
- Two player panels (four if you switch on 4-deck mode) with KEY SYNC, BEAT SYNC and MASTER, pads, CUE and PLAY rings, SLIP, Q and MT
- A rekordbox-style tempo ring: the jog ring is a round tempo fader. Drag it to change tempo, right-click to reset. The red arc shows the offset, and the ±N label under the BPM cycles the range (±6, 8, 10, 16, 24, 50 %)
- A track header with artist, the track's own BPM and key, elapsed and total time, and the current key with its colour bar between the key-shift arrows
- Pads that switch between Hot Cue, Beat Loop, Beat Jump and Loop Roll (click the mode name; right-click goes back). They default to 4 rows × 2 columns like rekordbox; the **2 COL / 4 COL** button next to the mode name switches to 2 rows × 4 columns, and the choice is remembered
- A centre mixer, effect units with a colour-FX row, mic and headphone controls, 16 samplers and a themed library

The FX panel is hidden at first. Turn it on with the FX button in the top bar.

## What's different from the real thing

- Hotcue pads fill completely with the cue colour, and there are no cue times. Mixxx doesn't allow anything fancier.
- There's no GROOVE CIRCUIT, MIX POINT LINK, STEMS or lighting panel, since Mixxx has nothing to hook them to.
- There's no separate tempo fader. The jog ring does that job, as in rekordbox.
- The jog doesn't scratch or spin. Mixxx draws its spinning platter in an OpenGL window that would cover the BPM readout and tempo ring.

## Heads up

I tested it in a real Mixxx under a virtual display, and this version was also checked on macOS (Apple Silicon). Linux and Windows on a real GPU haven't been checked yet. If something looks off, please open an issue.

## License

CC BY-SA 4.0. Rekordbox is a trademark of AlphaTheta Corporation. This project is independent and not affiliated with them, and all artwork here is original.
