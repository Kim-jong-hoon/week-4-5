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

## 🧪 설치 및 기본 사용법 (Python)

### ✅ 설치
```bash
pip install ultralytics
