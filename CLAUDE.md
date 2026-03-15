# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a single-page spelling game for a child named Ruby. The entire app lives in `index.html` — a self-contained HTML file with inline CSS and JavaScript (no build tools, no dependencies, no framework).

## How It Works

1. An admin enters 10 spelling words (one per line) in a textarea
2. The game reads each word aloud using the Web Speech API (`SpeechSynthesisUtterance`)
3. The child types the spelling and submits; correct answers are rewarded with a joke before advancing
4. Incorrect answers prompt a retry and re-read the word
5. After all 10 words are spelled correctly, a completion screen is shown

## Development

Open `index.html` directly in a browser (also served via GitHub Pages) — no server or build step required. To test speech synthesis, use a browser that supports the Web Speech API (Chrome, Safari, Edge).
