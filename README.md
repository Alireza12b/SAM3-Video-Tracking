# SAM 3 — Open-Vocabulary Video Tracking

Track a single moving target in a short video using only a text prompt, with Meta's
**Segment Anything Model 3 (SAM 3)**. The notebook segments the target, tracks it across every
frame, computes its centroid per frame, draws the motion path, and plots the trajectory.


## Requirements
- Google Colab with a **GPU** runtime
- The `sam3.pt` checkpoint

## How to run
Open `sam3_video_tracking.ipynb` in Colab and run the cells top to bottom:
1. **Setup** — checks the GPU and installs SAM 3.
2. **Checkpoint** — downloads `sam3.pt` and loads the model.
3. **Video** — upload your 5-second MP4.
4. **Prompts** — set the target concepts (default `["person", "bicycle"]`).
5. **Track** — runs SAM 3, computes centroids, renders the video, and plots the trajectory.

## Notes
- To track a different object, change `TEXT_PROMPTS`.
