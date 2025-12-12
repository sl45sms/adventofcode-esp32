# Advent of Code on ESP32
Just for fun the advent of code challenge (day_1) implemented on an ESP32 with a rotary encoder and a 7-segment display.

* Waveshare ESP32-S3-Matrix development board is used for this project.

## Input Data
I've use this python oneliner to generate the rotations array from the input data:
```
python - <<'PY'
from pathlib import Path
p = Path('input')
lines = p.read_text().replace('L','-').replace('R','').splitlines()
p.write_text(''.join(f"{line}," for line in lines))
PY
```
