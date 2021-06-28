# "Subtitles to Speech" and "FFMpeg combines video and audio"

## Prerequites

- get ready google cloud service confidentials under free tier limits, please see https://cloud.google.com/text-to-speech
- `python3` and `pip`
- `ffmpeg`, `ffmpeg-python`, `pydub`, `google-cloud-texttospeech==1.0.1`

```bash
# apt update
# apt install ffmpeg
# pip install ffmpeg-python
# pip install pydub pysrt google-cloud-texttospeech==1.0.1 
```

## Get Started

### Subtitles to Speech

- `srt_to_gcs_tts.ipynb`
  - use `pysrt` to parse the time in `.srt` subtitile files, and then call `google cloud services text-to-service` for each subtitle.
  - please make sure your google confidential is consistent to the path (`os.environ['GOOGLE_APPLICATION_CREDENTIALS'] = "../googlecloud.json"`)

###  FFMpeg combines video and audio

- `ffmpeg_combine.ipynb`
  - use `ffmpeg` to combine original video and google-tts generated audio.
