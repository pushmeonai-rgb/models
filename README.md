# faster-whisper-small (Systran) — copia para transcribir reels

Modelo `Systran/faster-whisper-small` (licencia MIT), partido en pedazos de 9 MB para poder subirlo a GitHub.

Rearmar:

```bash
git clone --depth 1 https://github.com/pushmeonai-rgb/models.git
cd models
cat model.bin.part-* > model.bin
sha256sum -c model.bin.sha256
```

Usar:

```python
from faster_whisper import WhisperModel
m = WhisperModel("models", device="cpu", compute_type="int8")
```
