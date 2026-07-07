# Smoke Generation Notes

Generated on 2026-07-06.

## Environment

- Virtualenv: `.venv-tts`
- GPU runtime verified with PyTorch `2.11.0+cu128` on NVIDIA B200 MIG.
- Model repos cloned under `models/`.

## Generated Outputs

- VoxCPM2: 14/14 tasks generated.
- VieNeu-TTS: 2/2 Vietnamese specialist tasks generated.
- JaiTTS-F5TTS: 2/2 Thai specialist tasks generated.

## Important Caveats

- Target text files are smoke-test scripts, not ASR-derived final translations.
- JaiTTS reference transcripts are approximate; use exact transcripts for final evaluation.
- Duration control was not tuned. Current outputs should be judged first for pronunciation, naturalness, and speaker similarity.
- VieNeu and JaiTTS required monkeypatching audio loading to avoid `torchaudio -> torchcodec` issues in this CUDA 12.8 / PyTorch 2.11 environment.

## Re-run Commands

```bash
. .venv-tts/bin/activate
HF_HUB_DISABLE_XET=1 python scripts/run_voxcpm_smoke.py
HF_HUB_DISABLE_XET=1 python scripts/run_vieneu_smoke.py
PYTHONPATH=models/thonburian-tts HF_HUB_DISABLE_XET=1 python scripts/run_jaitts_smoke.py
python scripts/check_smoke_outputs.py > results/metadata/smoke_output_check.csv
```
