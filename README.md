# YOLO v8과 YOLO v11 버전 영상의 FPS 차이
## YOLO v8 버전 일 때 fps
<img width="421" height="178" alt="dfdf" src="https://github.com/user-attachments/assets/0d7957bc-d538-42da-83c8-eb53f3b91d03" />

## YOLO v11 버전 일 떄 fps
<img width="347" height="152" alt="v11 영상 fps" src="https://github.com/user-attachments/assets/f0de9321-a4fb-42f9-9fa9-440c17ca980f" />



# 🔍 YOLOv11 by Ultralytics - Overview & Usage

> 최신 YOLO 시리즈인 **YOLOv11**은 Ultralytics에서 공식 출시한 모델로, 성능과 효율성을 모두 향상시킨 객체 탐지 모델입니다.

## 🚀 주요 특징

- 📦 **더 작고 빠른 모델**: YOLOv8 대비 파라미터 수 최대 22% 감소
- 🎯 **더 높은 정확도**: 향상된 mAP (mean Average Precision)
- 🧠 **다양한 백본 및 태스크 지원**:
  - Detection (탐지)
  - Segmentation (분할)
  - Pose Estimation (자세 인식)
  - Oriented Bounding Box (OBB)
  - Classification (분류)

## 📊 모델 사이즈 종류

| 모델 이름 | 설명 |
|-----------|------|
| `yolo11n.pt` | Nano (가장 가볍고 빠름) |
| `yolo11s.pt` | Small |
| `yolo11m.pt` | Medium |
| `yolo11l.pt` | Large |
| `yolo11x.pt` | Extra Large (가장 정확도 높음) |

각 사이즈별로 다음과 같은 태스크 지원 모델도 있습니다:
- `yolo11x.pt`, `yolo11x-seg.pt`, `yolo11x-pose.pt`, `yolo11x-obb.pt`, `yolo11x-cls.pt`

---

# 🔍 YOLOv12 – Attention-Centric Real‑Time Object Detector

Ultralytics 공식 최신 YOLO 시리즈 **YOLOv12**는 주목 기반(Attention-centric) 아키텍처를 도입해 **속도와 정확도 모두 업그레이드**된 모델입니다.

---

## 🚀 주요 특징

- **Attention‑centric 구조**: Area Attention, R‑ELAN, FlashAttention 최적화로 실시간 성능과 고정밀 mAP 달성 :contentReference[oaicite:1]{index=1}  
- **다양한 태스크 지원**: 회전 바운딩 박스(OBB), 분할(seg), 자세(pose), 분류(cls) 모두 가능 :contentReference[oaicite:2]{index=2}  
- **효율적 구조 개선**:
  - 파라미터 최적화, positional encoding 제거, FlashAttention 사용
  - CNN과의 하이브리드 방식으로 향상된 효율성 :contentReference[oaicite:3]{index=3}

---

## 📊 성능 벤치마크 (COCO val2017, 640px)

| 모델 | mAP (50–95) | GPU 지연(T4‑TensorRT FP16) | 파라미터(M) | FLOPs(B) | 전 버전 대비 |
|------|-------------|-----------------------------|-------------|----------|-------------|
| YOLO12n | 40.6% | 1.64 ms | 6.5 | — | +2.1 mAP vs YOLOv10n / +1.2 vs YOLOv11n :contentReference[oaicite:4]{index=4} |
| YOLO12s | 48.0% | 2.61 ms | 21.4 | — | +1.5 mAP vs RT‑DETR, +42% 속도 :contentReference[oaicite:5]{index=5} |
| YOLO12m | 52.5% | 4.86 ms | — | 67.5B | +1.0 mAP vs YOLO11m :contentReference[oaicite:6]{index=6} |
| YOLO12l | 53.7% | 6.77 ms | — | 88.9B | +0.4 mAP vs YOLO11l :contentReference[oaicite:7]{index=7} |
| YOLO12x | 55.2% | 11.79 ms | — | 199B | +0.6 mAP vs YOLO11x :contentReference[oaicite:8]{index=8} |

---


