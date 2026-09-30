---
name: AI update README
description: Make a small test change to the README and open a pull request

on:
  workflow_dispatch:

permissions:
  contents: read
  copilot-requests: write

engine:
  id: copilot
  model: gpt-5

safe-outputs:
  create-pull-request:
    max: 1
---

# AI Update README

Modify `README.md`.

Add this section at the end of the file:

## Status

This change was made by an AI agent.

Do not modify any other files.

After making the change, create a pull request against `main` containing the change.
