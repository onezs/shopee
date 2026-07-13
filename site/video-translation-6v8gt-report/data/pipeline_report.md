# Pipeline Report

Run dir: `video_trans_pipeline/runs/full-th-11110222-6v8gt-clean-mute-20260713`
Input video: `video_trans_pipeline/inputs/th-11110222-6v8gt-mq1q2eeg6hvk78.mp4`
Input SHA-256: `c2d63970c973668d3e5acbf0860ee9ad4ef3248fa3bce8060c708195100ca532`
Pipeline elapsed: `872.18s`

## Video

- Frames: `416`
- FPS: `25.0`
- Size: `540x960`
- Duration: `16.64s`

## Stages

| stage | status | elapsed | output |
| --- | --- | ---: | --- |
| source | completed | 0.43s | `video_trans_pipeline/runs/full-th-11110222-6v8gt-clean-mute-20260713/00_source/th-11110222-6v8gt-mq1q2eeg6hvk78.mp4` |
| extract_audio | completed | 1.07s | `video_trans_pipeline/runs/full-th-11110222-6v8gt-clean-mute-20260713/05_audio/source_audio.wav` |
| reference | completed | 0.49s | `video_trans_pipeline/runs/full-th-11110222-6v8gt-clean-mute-20260713/05_audio/reference.wav` |
| asr | completed | 47.00s | `video_trans_pipeline/runs/full-th-11110222-6v8gt-clean-mute-20260713/10_asr/source_segments.json` |
| translate | completed | 4.96s | `video_trans_pipeline/runs/full-th-11110222-6v8gt-clean-mute-20260713/20_translate/target_segments.json` |
| tts | completed | 249.37s | `video_trans_pipeline/runs/full-th-11110222-6v8gt-clean-mute-20260713/30_tts/tts_segments.json` |
| align_audio | completed | 0.24s | `video_trans_pipeline/runs/full-th-11110222-6v8gt-clean-mute-20260713/30_tts/full_tts.wav` |
| mix_audio | completed | 0.18s | `video_trans_pipeline/runs/full-th-11110222-6v8gt-clean-mute-20260713/35_mix/mixed_audio.wav` |
| ocr_detect | completed | 143.27s | `video_trans_pipeline/runs/full-th-11110222-6v8gt-clean-mute-20260713/40_ocr/det/detections.jsonl` |
| build_mask | completed | 12.97s | `video_trans_pipeline/runs/full-th-11110222-6v8gt-clean-mute-20260713/45_mask/mask.mp4` |
| eraserdit | completed | 410.81s | `video_trans_pipeline/runs/full-th-11110222-6v8gt-clean-mute-20260713/50_erase/erased_video.mp4` |
| mux | completed | 0.83s | `video_trans_pipeline/runs/full-th-11110222-6v8gt-clean-mute-20260713/60_mux/final.mp4` |

## OCR Detection

- Processed FPS: `2.9892237752337696`
- Positive frames: `416`
- Total boxes: `1248`
- Avg boxes/frame: `3.0`

## Mask QA

- Frames written: `416`
- Positive mask ratio: `100.00%`
- Empty mask runs: `[]`
- Avg coverage: `7.97%`
- P95 coverage: `8.21%`
- Max coverage: `8.39%`
- Persistence enabled: `True`
- Persistence frames: `10`
- Persistence rois: `['bottom', 'middle', 'top']`
- Tracking enabled: `False`
- Track count: `n/a`
- Interpolated boxes: `n/a`

## Text Segments

| id | time | source | target |
| --- | ---: | --- | --- |
| seg_0000 | 0.00-1.40 | Lip Maybelline White New Ink | Son Maybelline Vinyl Ink |
| seg_0001 | 1.40-3.70 | ป้ายยาลิปโทนนูสสวยหวานละมุนนูโทโท | Gợi ý dòng son tông nude ngọt ngào, dịu dàng |
| seg_0002 | 3.70-5.90 | เปอร์หนึ่งสูญสวน นูสชมพูอมพีชนิดนิด | Màu 100, tông nude hồng pha chút ánh đào |
| seg_0003 | 5.90-7.90 | เป็นอีกหนึ่งสีที่มีไว้ได้ใช้บ่อยแน่นอน | Đây chắc chắn là màu son bạn sẽ dùng rất thường xuyên |
| seg_0004 | 7.90-10.20 | เหนือลิปให้สีสวยชัด ปากชื่นชื้นฉ่ำว้าว | Chất son lên màu chuẩn, môi căng mọng ẩm mượt |
| seg_0005 | 10.20-11.90 | รุ่นนี้เขาขึ้นชื่อเรื่องความติดโทนเลย | Dòng này nổi tiếng siêu lâu trôi luôn |
| seg_0006 | 11.90-14.40 | สิ่งที่เห็นในตะกร้าต้องรีบกดนะ ของหมดไปมาก | Thấy trong giỏ hàng là phải chốt ngay, nhanh hết lắm |
| seg_0007 | 14.40-16.60 | ตอนนี้มีโปรด้วยนะพี่กับใต้คลิปเลยค่ะ | Đang có ưu đãi đó, nhấn vào link dưới clip nha |

## TTS Alignment

- Target duration: `16.64s`
- Segments: `8`
- Overrun count: `5`
- Shift conflict count: `1`

| id | source window | tts duration | scheduled | status |
| --- | ---: | ---: | ---: | --- |
| seg_0000 | 0.00-1.40 | 1.76s | 0.00-1.76 | overrun |
| seg_0001 | 1.40-3.70 | 2.40s | 1.40-3.80 | ok |
| seg_0002 | 3.70-5.90 | 2.40s | 3.85-6.25 | shift_conflict |
| seg_0003 | 5.90-7.90 | 2.56s | 5.90-8.46 | overrun |
| seg_0004 | 7.90-10.20 | 2.72s | 7.90-10.62 | overrun |
| seg_0005 | 10.20-11.90 | 2.08s | 10.20-12.28 | overrun |
| seg_0006 | 11.90-14.40 | 2.40s | 11.90-14.30 | ok |
| seg_0007 | 14.40-16.60 | 2.72s | 14.40-17.12 | overrun |

## Audio Mix

- Output: `video_trans_pipeline/runs/full-th-11110222-6v8gt-clean-mute-20260713/35_mix/mixed_audio.wav`
- Duration: `16.64s`
- Original audio muted: `True`
- Background mode: `silence`
- Ducking source: `tts_schedule`
- BGM gain: `-3.0 dB`
- Ducking gain: `-10.0 dB`

## Outputs

- `source_video`: `video_trans_pipeline/runs/full-th-11110222-6v8gt-clean-mute-20260713/00_source/th-11110222-6v8gt-mq1q2eeg6hvk78.mp4`
- `source_audio`: `video_trans_pipeline/runs/full-th-11110222-6v8gt-clean-mute-20260713/05_audio/source_audio.wav`
- `vocals_audio`: `video_trans_pipeline/runs/full-th-11110222-6v8gt-clean-mute-20260713/05_audio/source_audio.wav`
- `background_audio`: `video_trans_pipeline/runs/full-th-11110222-6v8gt-clean-mute-20260713/05_audio/source_audio.wav`
- `reference_wav`: `video_trans_pipeline/runs/full-th-11110222-6v8gt-clean-mute-20260713/05_audio/reference.wav`
- `detections_jsonl`: `video_trans_pipeline/runs/full-th-11110222-6v8gt-clean-mute-20260713/40_ocr/det/detections.jsonl`
- `mask_video`: `video_trans_pipeline/runs/full-th-11110222-6v8gt-clean-mute-20260713/45_mask/mask.mp4`
- `erased_video`: `video_trans_pipeline/runs/full-th-11110222-6v8gt-clean-mute-20260713/50_erase/erased_video.mp4`
- `source_segments`: `video_trans_pipeline/runs/full-th-11110222-6v8gt-clean-mute-20260713/10_asr/source_segments.json`
- `target_segments`: `video_trans_pipeline/runs/full-th-11110222-6v8gt-clean-mute-20260713/20_translate/target_segments.json`
- `tts_manifest`: `video_trans_pipeline/runs/full-th-11110222-6v8gt-clean-mute-20260713/30_tts/tts_segments.json`
- `full_tts_audio`: `video_trans_pipeline/runs/full-th-11110222-6v8gt-clean-mute-20260713/30_tts/full_tts.wav`
- `mixed_audio`: `video_trans_pipeline/runs/full-th-11110222-6v8gt-clean-mute-20260713/35_mix/mixed_audio.wav`
- `final_video`: `video_trans_pipeline/runs/full-th-11110222-6v8gt-clean-mute-20260713/60_mux/final.mp4`
