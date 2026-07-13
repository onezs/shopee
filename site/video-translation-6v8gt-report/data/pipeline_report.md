# Pipeline Report

Run dir: `/home/work/opa_common/zhanghaoran/video_trans_pipeline/runs/full-th-11110222-6v8gt-vision-001`
Input video: `/home/work/opa_common/zhanghaoran/video_trans_pipeline/inputs/th-11110222-6v8gt-mq1q2eeg6hvk78.mp4`
Pipeline elapsed: `450.49s`

## Video

- Frames: `416`
- FPS: `25.0`
- Size: `540x960`
- Duration: `16.64s`

## Stages

| stage | status | elapsed | output |
| --- | --- | ---: | --- |
| source | skipped_cached | 0.00s | `/home/work/opa_common/zhanghaoran/video_trans_pipeline/runs/full-th-11110222-6v8gt-vision-001/00_source/th-11110222-6v8gt-mq1q2eeg6hvk78.mp4` |
| extract_audio | skipped_cached | 0.00s | `/home/work/opa_common/zhanghaoran/video_trans_pipeline/runs/full-th-11110222-6v8gt-vision-001/05_audio/source_audio.wav` |
| reference | skipped_cached | 0.00s | `/home/work/opa_common/zhanghaoran/video_trans_pipeline/runs/full-th-11110222-6v8gt-vision-001/05_audio/reference.wav` |
| asr | completed | 51.66s | `/home/work/opa_common/zhanghaoran/video_trans_pipeline/runs/full-th-11110222-6v8gt-vision-001/10_asr/source_segments.json` |
| translate | completed | 4.30s | `/home/work/opa_common/zhanghaoran/video_trans_pipeline/runs/full-th-11110222-6v8gt-vision-001/20_translate/target_segments.json` |
| tts | completed | 389.32s | `/home/work/opa_common/zhanghaoran/video_trans_pipeline/runs/full-th-11110222-6v8gt-vision-001/30_tts/tts_segments.json` |
| align_audio | completed | 0.29s | `/home/work/opa_common/zhanghaoran/video_trans_pipeline/runs/full-th-11110222-6v8gt-vision-001/30_tts/full_tts.wav` |
| mix_audio | completed | 0.20s | `/home/work/opa_common/zhanghaoran/video_trans_pipeline/runs/full-th-11110222-6v8gt-vision-001/35_mix/mixed_audio.wav` |
| ocr_detect | skipped_cached | 0.00s | `/home/work/opa_common/zhanghaoran/video_trans_pipeline/runs/full-th-11110222-6v8gt-vision-001/40_ocr/det/detections.jsonl` |
| build_mask | skipped_cached | 0.00s | `/home/work/opa_common/zhanghaoran/video_trans_pipeline/runs/full-th-11110222-6v8gt-vision-001/45_mask/mask.mp4` |
| eraserdit | skipped_cached | 0.00s | `/home/work/opa_common/zhanghaoran/video_trans_pipeline/runs/full-th-11110222-6v8gt-vision-001/50_erase/erased_video.mp4` |
| mux | completed | 4.01s | `/home/work/opa_common/zhanghaoran/video_trans_pipeline/runs/full-th-11110222-6v8gt-vision-001/60_mux/final.mp4` |

## OCR Detection

- Processed FPS: `1.7593960893975265`
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
| seg_0000 | 0.00-1.38 | Lip Maybelline White New Ink | Son Maybelline Vinyl Ink |
| seg_0001 | 1.38-3.72 | ป้ายยาลิปโทนนูตสวยหวานละมุนนูตโทโท | Gợi ý thỏi son tông nude ngọt ngào, dịu dàng cực xinh. |
| seg_0002 | 3.72-5.76 | เปอร์หนึ่งสูญส่วนนูตชมพูอมพีชนิดนิด | Màu số 10, tông nude hồng pha chút cam đào. |
| seg_0003 | 5.76-7.74 | เป็นอีกหนึ่งสีที่มีไว้ได้ใช้บ่อยแน่นอน | Đây chắc chắn là màu son bạn sẽ dùng rất thường xuyên. |
| seg_0004 | 7.74-10.14 | เหนือลิปให้สีสวยชัดปากชื่นชื้นชำวาว | Chất son lên màu chuẩn, dưỡng ẩm cho môi căng bóng. |
| seg_0005 | 10.14-11.90 | รุ่นนี้เขาขึ้นชื่อเรื่องความติดโทนเลย | Dòng này nổi tiếng siêu lâu trôi luôn đó. |
| seg_0006 | 11.90-14.38 | สิ่งที่เห็นในตะกร้าต้องรีบกดนะ ของหมดไปมาก | Thấy trong giỏ hàng là phải chốt ngay, nhanh hết lắm. |
| seg_0007 | 14.38-16.62 | ตอนนี้มีโปรด้วยนะพี่กับใต้คลิปเลยค่ะ | Đang có ưu đãi nữa đó, nhấn vào dưới clip nha. |

## TTS Alignment

- Target duration: `16.64s`
- Segments: `8`
- Overrun count: `8`
- Shift conflict count: `0`

| id | source window | tts duration | scheduled | status |
| --- | ---: | ---: | ---: | --- |
| seg_0000 | 0.00-1.38 | 1.76s | 0.00-1.76 | overrun |
| seg_0001 | 1.38-3.72 | 3.84s | 1.38-5.22 | overrun |
| seg_0002 | 3.72-5.76 | 3.04s | 3.72-6.76 | overrun |
| seg_0003 | 5.76-7.74 | 3.20s | 5.76-8.96 | overrun |
| seg_0004 | 7.74-10.14 | 3.36s | 7.74-11.10 | overrun |
| seg_0005 | 10.14-11.90 | 2.56s | 10.14-12.70 | overrun |
| seg_0006 | 11.90-14.38 | 4.00s | 11.90-15.90 | overrun |
| seg_0007 | 14.38-16.62 | 3.36s | 14.38-17.74 | overrun |

## Audio Mix

- Output: `/home/work/opa_common/zhanghaoran/video_trans_pipeline/runs/full-th-11110222-6v8gt-vision-001/35_mix/mixed_audio.wav`
- Duration: `16.64s`
- Ducking source: `tts_schedule`
- BGM gain: `-3.0 dB`
- Ducking gain: `-10.0 dB`

## Outputs

- `source_video`: `/home/work/opa_common/zhanghaoran/video_trans_pipeline/runs/full-th-11110222-6v8gt-vision-001/00_source/th-11110222-6v8gt-mq1q2eeg6hvk78.mp4`
- `source_audio`: `/home/work/opa_common/zhanghaoran/video_trans_pipeline/runs/full-th-11110222-6v8gt-vision-001/05_audio/source_audio.wav`
- `vocals_audio`: `/home/work/opa_common/zhanghaoran/video_trans_pipeline/runs/full-th-11110222-6v8gt-vision-001/05_audio/source_audio.wav`
- `background_audio`: `/home/work/opa_common/zhanghaoran/video_trans_pipeline/runs/full-th-11110222-6v8gt-vision-001/05_audio/source_audio.wav`
- `reference_wav`: `/home/work/opa_common/zhanghaoran/video_trans_pipeline/runs/full-th-11110222-6v8gt-vision-001/05_audio/reference.wav`
- `detections_jsonl`: `/home/work/opa_common/zhanghaoran/video_trans_pipeline/runs/full-th-11110222-6v8gt-vision-001/40_ocr/det/detections.jsonl`
- `mask_video`: `/home/work/opa_common/zhanghaoran/video_trans_pipeline/runs/full-th-11110222-6v8gt-vision-001/45_mask/mask.mp4`
- `erased_video`: `/home/work/opa_common/zhanghaoran/video_trans_pipeline/runs/full-th-11110222-6v8gt-vision-001/50_erase/erased_video.mp4`
- `source_segments`: `/home/work/opa_common/zhanghaoran/video_trans_pipeline/runs/full-th-11110222-6v8gt-vision-001/10_asr/source_segments.json`
- `target_segments`: `/home/work/opa_common/zhanghaoran/video_trans_pipeline/runs/full-th-11110222-6v8gt-vision-001/20_translate/target_segments.json`
- `tts_manifest`: `/home/work/opa_common/zhanghaoran/video_trans_pipeline/runs/full-th-11110222-6v8gt-vision-001/30_tts/tts_segments.json`
- `full_tts_audio`: `/home/work/opa_common/zhanghaoran/video_trans_pipeline/runs/full-th-11110222-6v8gt-vision-001/30_tts/full_tts.wav`
- `mixed_audio`: `/home/work/opa_common/zhanghaoran/video_trans_pipeline/runs/full-th-11110222-6v8gt-vision-001/35_mix/mixed_audio.wav`
- `final_video`: `/home/work/opa_common/zhanghaoran/video_trans_pipeline/runs/full-th-11110222-6v8gt-vision-001/60_mux/final.mp4`
