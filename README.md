# Personal Dashboard

A single-file dashboard with a clock, live weather, to-dos, bookmarks, and notes. Everything saves to your browser's localStorage, so it works fully offline. Live at [rickysend.github.io/dashboard/](https://rickysend.github.io/dashboard/).

## Why I built it

I wanted one page to open when I start the browser — a home for the small tools I use every day. I built it with an AI coding agent in one evening, guided by a rules file I had written after watching the agent repeat a mistake. The point of the project was never the features; it was learning to direct an agent and check its work.

## What I learned

The to-dos did not survive a refresh. I checked localStorage in DevTools and could see the data was being saved, which narrowed the bug to loading rather than saving — the save handler and the load-on-startup line were out of step. That has become the pattern I use for everything now: verify the data first, then explain what I ruled out.