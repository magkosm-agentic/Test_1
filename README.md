# The Paperclip Protocol

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
| `A` | autoplay, paced to about 5½ minutes |
| `T` | jump to the debrief slide (what was real, what was invented) |
| `R` | restart and reset the clock |
| `F` | fullscreen |
| `?` | key help |

The clock in the bottom-right starts on your first advance and turns red past six minutes.

## Structure

1. Cover
2. Peenemünde, 3 October 1942: the V-2 reaches 84.5 km
3. The weapon: 3,000 fired, 9,000 killed, 12,000 dead building it
4. The vanishing: Zhukov, Stalin and the FBI file
5. Two boats: U-530 and U-977 reach Argentina
6. The skull: the 2009 DNA result and Operation Archive
7. Paperclip: von Braun, Debus, Rudolph, Strughold
8. The novel: "Elon"
9. The race: Sputnik to the N1
10. Six landings, one side: Apollo, Project A119, Project Horizon
11. December 1972 to January 2019: 16,821 days
12. Pull the thread
13. The quietest place
14. Debrief (hidden; press `T`)

Edit the text directly in the HTML. Each slide is a `<section class="slide">`; anything with
`class="frag"` reveals on the next keypress; `data-dur` is the slide's autoplay length in seconds;
the `<aside class="notes">` is what the `N` panel shows.
