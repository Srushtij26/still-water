# Still Water

A calming pond game. Touch the water to play notes, feed the fish and watch them grow,
and let the seasons and the day and night cycle drift by.

## Features
- Four seasons (Spring, Summer, Autumn, Winter), each with its own colours, scale, drone and falling petals, fireflies, leaves or snow
- A day and night cycle with a different look in every season: a sun and moon, stars, warm or cool dusk glow, and an aurora in winter. A button moves time forward
- Rain with synthesised rain sound
- Nine kinds of fish (koi, goldfish, ghost koi, shubunkin, kohaku, ogon, veiltail, neon school, platinum) that grow up to twice their size when fed
- Generative music, plus a breathing guide

All sound is synthesised in the browser with the Web Audio API, so there are no audio files.

## Run locally
    pip install -r requirements.txt
    python app.py        # http://localhost:5000

## Deploy
Flask serves one static page, so any Python host works.
- **Render / Railway / Fly.io:** connect the repo. Build command `pip install -r requirements.txt`, start command `gunicorn app:app`. The Procfile is included.
- **PythonAnywhere:** point the WSGI file at `app:app`.
