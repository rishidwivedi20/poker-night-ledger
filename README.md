# Poker Night Ledger

A mobile-first chip tracker for home poker games. You deal the physical cards; the app keeps every chip, blind, pot, side pot and payout straight.

Single file, no build step, no dependencies. Open `index.html` in a browser, or serve the repo with GitHub Pages.

## Features

- **Stakes you control:** buy-in, small and big blind, ante, rebuy amount, and optional blinds that double every N hands.
- **Full betting engine:** check, call, bet, raise with the minimum-raise rule, all-in, short all-ins that do not reopen raising, uncalled bets returned, and side pots.
- **Showdown:** pick the winner of each pot, or split a pot between several players.
- **Table management:** sit out, add late players, rebuy any time between hands (or when folded), and choose who deals next.
- **Settle up:** set what one chip is worth and get the fewest payments needed to clear the night. Copy the results to share.
- **History and standings:** hand log, biggest pot, podium, net result per player.
- **Oval table or list:** automatic for up to 6 players, switchable under Rules.
- **Undo** for any action, plus sound and vibration that you can switch off.
- **Saves on your device** with `localStorage`, so a reload or closed tab never loses the game.

## Run it

```sh
open index.html          # or double-click it
# or serve it
python3 -m http.server 8000
```

To publish with GitHub Pages: Settings, Pages, deploy from the `main` branch root.

## Notes

- Everything is stored in the browser on the device you play on. A different phone starts fresh.
- Fonts (Bodoni Moda and Manrope) load from Google Fonts. Without a connection the app falls back to system fonts.

## Rules covered

Texas Hold'em betting rounds (preflop, flop, turn, river), heads-up blind positions, blinds and antes, minimum raises, side pots, and odd chips in split pots going to the winner nearest the dealer's left.
