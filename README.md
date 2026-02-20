# Destiny Activity Compiler

A command-line C++ application that retrieves a player's recent Destiny 2 activity history using the Bungie API and exports it to a CSV file.

---

## Overview

Destiny Activity Compiler is designed to:

- Retrieve a player's activity history from the Bungie API
- Compile activity data into a structured CSV file
- Serve as a backend foundation for a future GUI-based application

The program currently runs as a standalone CLI tool, but it is structured to be integrated into a larger application later.

---

## Features

- Search player by Bungie Name (e.g. `Char#5202`)
- Automatically detects correct platform membership
- Retrieves recent activity data
- Outputs results to `activities.csv`
- Includes:
  - Activity date
  - Activity duration
  - Link to the official Bungie PGCR (Post Game Carnage Report)

---

## Requirements

- C++17 or newer
- libcurl
- nlohmann/json (single header version)
- A valid Bungie API key

---

## Build Instructions

### Option 1 — Compile with API Key as Macro

```bash
g++ -std=c++17 tracker.cpp -o tracker -lcurl -DBUNGIE_API_KEY="\"your_key_here\""
