# Repository Guidance

This file provides guidance to code assistants working in the `samune-maker` repository.

## Project Overview

This repository contains a small thumbnail maker web app. The app renders a base image and allows the user to place editable text layers over it. Text layers support font selection, color, outline, alignment, and layout within a canvas-based region.

## Architecture

- **Single-page static app**: Everything lives in `index.html` with embedded CSS and JavaScript
- **Canvas rendering**: Uses the HTML5 Canvas API for image drawing and text rendering
- **Layered text editing**: Supports multiple text layers with independent styling and positioning
- **Export**: Can download the rendered canvas as a PNG image
- **State save/load**: Supports exporting/importing editor state as JSON

## Important Files

- `index.html` — main application file
- `README.md` — project description and usage notes

## Development Notes

- No build step is required; open `index.html` directly in a browser to run the app
- The editor handles image drag-and-drop, text alignment, and outline styling
- JSON state import/export is available to preserve the current background and text layer settings
- Keep changes focused on the single-file app and avoid adding unnecessary build tooling or extra dependencies
