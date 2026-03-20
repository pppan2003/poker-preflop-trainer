# Poker Preflop Trainer

A single-file web app for drilling GTO preflop ranges for 8-max cash games, based on 千算大學 range charts.

## Features

- **手牌練習** — Flash-card style: given a scenario + hand, choose the correct action
- **格子練習** — Paint the full 13×13 hand matrix using drag-to-paint, then submit for feedback
  - ⚠️ Partial credit for overlapping actions (e.g. picked Raise but correct is Raise/Call)
  - ❌ Wrong for completely incorrect actions
  - Live range % counter (mixed actions count as 0.5)
- **範圍表** — Browse all 89 scenarios as color-coded 13×13 matrices
- **統計** — Track accuracy per scenario; view Top-10 mistake hands; launch targeted weakness drills
- **弱點練習** — Automatically jumps to the scenario with your most-missed hands, highlighted in gold

## Data

89 GTO scenarios extracted from the 千算大學 8-max range Excel file, covering:
- Opening ranges (UTG → BB)
- ISO raises (single & double limper)
- Facing opens (all position combinations)
- Facing 3-bets
- IP/OOP special scenarios

## Usage

Open `gto_quiz.html` in any browser. No installation required. Progress is saved in localStorage.
