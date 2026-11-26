# Text-to-Video on Google Colab

I used Zeroscope v2 to generate a three-second video from a text prompt
on a free Google Colab Tesla T4 GPU.

[View the notebook](./text_to_video_colab.ipynb) · [Watch the video](./boat.mp4)

## Prompt

> A small yellow paper boat floats slowly from left to right across a
> shallow pond. Gentle ripples trail behind it. Fixed camera at water level.

## Result

The clip captures the yellow paper boat and rippling water. The boat
stays near the center, so the requested left-to-right motion is subtle.

## Experiment settings

| Setting | Value |
|---|---|
| Model | cerspense/zeroscope_v2_576w |
| GPU and precision | Tesla T4, FP16 |
| Resolution | 576 × 320 |
| Playback | 24 frames at 8 fps |
| Denoising steps | 25 |
| Seed | 42 |

## Run it yourself

Open the notebook in Google Colab, select a GPU runtime, and run the
cells in order. Change the prompt to generate a different scene.

[Model card and license](https://huggingface.co/cerspense/zeroscope_v2_576w)
