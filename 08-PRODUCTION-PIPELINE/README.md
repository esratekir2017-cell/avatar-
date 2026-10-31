# VELORA 30-second commercial — production pipeline v1

## Source of truth
Canonical Esra avatar: `IMG_7316.jpeg`, OpenArt reference `5AnoW2agSbonaMWxQ8uK`. Short black bob/bangs, green-grey eyes, freckles and facial proportions remain locked. Never use the long-haired storyboard model as the main character.

## Workflow (no repeated questions)
1. Reuse approved reference image and original VELORA logo. Check assets and commercial rights.
2. Generate exactly three 10-second 16:9 1080p scenes: (1) helicopter + paparazzi + heroine arrival; (2) red lipstick product close-up; (3) handsome man approaches, sustained eye contact, VELORA ending.
3. **Identity gate:** inspect faces in each scene against IMG_7316 before accepting; reject face drift, wrong hairstyle, hand errors or illegible logo. Do not pretend this can be verified by FFmpeg.
4. **Asset gate:** download the three actual MP4s or accept direct user-uploaded originals. A storyboard slideshow is not a substitute. Do not claim access if network DNS fails.
5. **Assembly gate:** use FFmpeg with consistent 1920x1080, 24fps; trim scenes to 10s each, concat to 30s; optionally add licensed music and an original-logo overlay after source review.
6. **Technical gate:** ffprobe exact duration, resolution, codec, stream integrity, then inspect video playback and check the man/eye-contact scene is actually present.
7. Deliver **one playable MP4**, source manifest, and explicit review status.

## Automation limits
OpenArt generation and GitHub text updates are connected. Local FFmpeg works. OpenArt CDN downloads from the current container failed with DNS name resolution, so the source-video transfer remains a real integration blocker. A connected OpenArt generation record does not mean its MP4 is locally available. No free web app is assumed to provide an API. Do not automatically spend credits for repeated generations when a manual identity approval is pending.

## Local assembly
Run the supplied `assemble.py` with three approved local MP4s, ordered arrival/lipstick/encounter. The `--approved-avatar` flag is an operator assertion after visual review, not a facial recognition feature. The script blocks missing clips, wrong resolution, incorrect clip length, or missing identity approval. Final output must be reviewed before commercial use.

## Existing reference
OpenArt identity test history: `cRNrC5mT0kJtevIk0NRJ` (10s, not final 30s). Existing 3 historical 10s scenes are not approved as identity-consistent by default.
