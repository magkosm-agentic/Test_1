# Operation Paperclip

A self-contained animated slide deck for a conspiracy-night presentation: five and a half minutes
from the first V-2 flight at Peenemünde to the far side of the Moon. Every date in it is real;
the story lives in the gaps between them. A hidden debrief slide separates the two.

## Running it

Open `paperclip-protocol.html` in a modern browser (Chrome, Edge, Firefox, Safari). No build step,
no server. The stage is a fixed 1920×1080 canvas scaled to the window, so present it fullscreen (`F`).

| Key | Action |
| --- | --- |
| `→` `space` click | next step or slide |
| `←` | back |
| `N` | speaker notes with cue times |
| `A` | autoplay, paced to about 6½ minutes |
| `T` | jump to the debrief slide (what was real, what was invented) |
| `R` | restart and reset the clock |
| `F` | fullscreen |
| `?` | key help |

The clock in the bottom-right starts on your first advance and turns red past six and a half minutes.

## Photos

The deck uses sixteen historical photographs under `assets/`, all public domain or Bundesarchiv
CC BY-SA 3.0 DE, downscaled for presentation. `assets/IMAGES.md` lists each file, its Wikimedia
Commons source and its licence. Any slot whose file is missing renders as a labelled "archive photo,
not on file" card, so the deck presents cleanly with a partial set.

## Structure

1. Cover
2. The vehicles: V-2 and Saturn V to scale, and the two Vs
3. The cast: Hitler, Stalin, Dornberger, von Braun, Debus, Rudolph
3. Peenemünde, 3 October 1942: the V-2 reaches 84.5 km
4. The weapon: 3,000 fired, 9,000 killed, 12,000 dead building it underground
5. Hitler vanishes: Zhukov, Stalin and the FBI file
6. Two boats: U-530 and U-977 reach Argentina
7. The skull: the 2009 DNA result and Operation Archive
8. Paperclip: "They didn't lose the space race. They ran it."
9. The novel: "Elon"
10. The race: every time the Soviets got close, something broke
11. Six landings, one side: Apollo, Project A119, Project Horizon
12. Underground: Nordhausen, Argentina, Antarctica, and then up
13. December 1972 to January 2019: 16,821 days, "it was reserved"
14. Pull the thread
15. They went underground. Then they went up.
16. Debrief (hidden; press `T`)

Colour rule: amber marks things on the record, red marks the claims we made up. Edit the text directly in the HTML. Each slide is a `<section class="slide">`; anything with
`class="frag"` reveals on the next keypress; `data-dur` is the slide's autoplay length in seconds;
the `<aside class="notes">` is what the `N` panel shows.
