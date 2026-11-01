# Zone ($ZONE)

A token launch agent on Solana with a 2000s internet look. You give it a name, a ticker and a link. Zone writes the contract, wires your 2% creator share and mints the token.

## Deploy
The site is a single `index.html` with no folders and no build step. Drop it into a GitHub repo or Vercel.

## Settings
Open `index.html` and find `CONFIG` near the top of the script:

```js
var CONFIG={xUrl:'',ca:'',buyUrl:'',chartUrl:''};
```

## What's on the page
- **Desktop hero:** a teal Win95-style desktop with pixel icons, a big ZONE.EXE coding terminal, and 8 monitor windows around it: contract.rs (syntax-highlighted code), compiler.log, tests.exe, deploy.log, mempool, fees.cfg (pie chart), explorer feed and netmon.
- **Working terminal:** type `launch` and answer the questions, or type `launch Name $TICKER` in one go. The agent streams the contract code, wires the 2% share, runs 12 tests and "mints" the token as a simulation, and every monitor reacts. Other commands: help, explore, status, fees, whoami, clear.
- **Rest of the page:** a live sample ticker bar, stats, an index of folders, features, how it works, an explorer of tokens (including "Yours"), a network monitor, the $ZONE token section, an FAQ and a call to action.
- **Taskbar:** a Start menu and taskbar at the bottom.

Everything on the page is a labelled simulation. The terminal sends nothing on-chain, and launched tokens are saved only on the visitor's device.
