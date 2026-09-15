# MLBB Coach V5 prototype

This is the first V5 working prototype.

## Included
- MLBB screenshot upload
- Game phase / role / hero context
- Live-style coaching UI
- Game-state model
- Gold, kills, towers and objective reasoning
- Fed-enemy and jungle-threat coaching
- Role-specific advice
- Demo mode

## Next V5 backend
The production pipeline should be:

Screenshot/video frame
-> MLBB vision/OCR
-> normalized GameState
-> temporal smoothing
-> strategy/recommendation engine
-> coaching events
-> UI

The browser build intentionally does not read game memory, intercept network traffic, inject taps, or automate gameplay.

## Video
Treat video as sampled frames for analysis. The next version can add frame extraction and send representative frames to the vision backend.

## Data
Patch-specific hero/build/counter data should be versioned and refreshed before live recommendations.
