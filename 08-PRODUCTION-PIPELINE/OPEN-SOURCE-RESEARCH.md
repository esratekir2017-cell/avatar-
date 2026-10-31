# VELORA open-source production research — 2026-10-31

## Official repositories reviewed
- ComfyUI: https://github.com/Comfy-Org/ComfyUI
- Wan 2.2 workflows: https://github.com/Comfy-Org/workflow_templates
- Wan 2.2 Animate character workflow: https://github.com/Comfy-Org/docs/blob/main/tutorials/video/wan/wan2-2-animate.mdx
- LTX Video/LTX-2: https://github.com/Lightricks/LTX-Video
- FFmpeg: https://github.com/FFmpeg/FFmpeg
- InsightFace: https://github.com/deepinsight/insightface (code license and pretrained model licenses differ; do not assume commercial model rights)

## Recommended architecture
OpenArt currently connected for generation; canonical avatar IMG_7316.jpeg reference; identity-gated scene approval; FFmpeg technical assembly and inspection; one 30-second MP4. ComfyUI + Wan Animate and LTX-2 are optional research tracks, not installed/automated systems. Validate GPU availability and all model-weight commercial licenses before use.

## QA gates
1. Same canonical face, short black bob/bangs, freckles and eyes; visual approval required.
2. Story contains helicopter, paparazzi, lipstick macro, handsome male approach, clearly visible mutual eye contact, VELORA ending.
3. Technical 16:9 1920x1080 24fps 30.0 seconds; audio, decoding and continuity checks.
4. Rights: original logo, commercially permitted weights, music and media.
5. Do not pass storyboard slideshow or a failed identity clip as final.

## Known integration blocker
Current container cannot download from cdn.openart.ai due to DNS resolution failure. FFmpeg is installed locally. Until original source MP4s are accessible, do not claim a finished assembled film.
