# v2-responsive-grid

v2-responsive-grid is an/my intended successor to [responsive-grid](https://github.com/nib-styles/responsive-grid)

See that repo for the basic gist of everything.

## Why?

The original responsive-grid system is limiting at certain breakpoints e.g You can only use 3rds @ 6 or 12 columns, you can't use quarters @ 6 or 10 etc. 

Also, the original system was also seemingly set up with arbitrary breakpoints based on no devices (as it clearly states in the readme). This means that our break points may not cater to an even spread of devices (i.e 50% are caught by 4, 30% by 12, why have any others?). This is something that should be, but is not currently, fixed by this solution.

## What's changed?

* All breakpoints now feature 12 columns, no exceptions. If you misuse them, it is your own fault (i.e it's probably not a good idea to use rg-1AtXs, but you might have some crazy requirements)

* Breakpoints have been renamed to Xs (4/1em), Sm (6/30em), Md (8/40em), Lg (12/60em) - bootstrap style, as they no longer represent the total columns available

* The 10 column (50em) breakpoint has been removed (as I believe there is not enough devices we support between 8 & 12 to justify having such a breakpoint, although I'm flexible on that). This saves some bytes for the client too

## Moving forward

I'd like to progress this towards a few things:

* Branching/creating a new component with just the new widths. This will allow us to use the old rg system along side the new widths

* Investigate better breakpoints, more specific to current devices

* Figure out a simpler way to migrate solutions using the original framework to this one

## Caveats

This uses a later version of SASS then what was original used (it has a map). Be a good dev and update your tools once in a while.





