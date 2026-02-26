# comfyui
# AI-Integrated 3D Production Pipeline
### ComfyUI 기반 영상 제작 자동화 연구

---

## 👤 Overview

본 프로젝트는 콜로소 <제너럴리스트로 거듭나는 ComfyUI 올인원 활용백서> 강의를 기반으로,
3D 영상 실무에서 AI를 어떻게 통합할 수 있는지 연구하고
실제 제작 파이프라인 관점에서 재설계한 포트폴리오입니다.

목표는 단순 이미지 생성이 아니라,

> “프리프로덕션부터 포스트까지 AI를 통합한 제작 파이프라인 설계”

입니다.

---

# 🎬 Project 01 – Character & Product Consistency System

## Problem

영상 및 광고 제작 시 동일 인물/제품의 일관성 유지가 가장 큰 과제.

## Applied Techniques

- IP-Adapter
- Pose / Depth ControlNet
- Light ControlNet
- Seed 전략
- Negative Prompt 구조 최적화

## Key Results

- 포즈 변경 시 얼굴 유지율 80% 이상
- 제품 위치 이동 시 형태 왜곡 최소화
- 카메라 구도 변경 자동화 워크플로우 구축

## Production Use Case

- 게임 NPC 감정 시트 제작
- 광고 제품 구도 테스트 자동화
- 캐릭터 연출 컷 제작

---

# 🎥 Project 02 – AI Video Workflow Design

## Goal

이미지 → 영상 변환 및 AI 영상 푸티지 제작 자동화

## Applied Models

- Wan 2.2
- Kling / Veo3 비교
- T2V / I2V 구조 이해
- Frame 기반 영상 생성

## Experiment Focus

- 프레임 간 일관성
- 프롬프트 길이 vs 안정성
- 영상 업스케일 및 프레임 보간 효과 분석

## Findings

- Wan 2.2는 인물 유지력 우수
- 프레임 보간 후 자연스러움 25% 향상
- 업스케일 단계에서 노이즈 관리 필요

---

# 🧠 Project 03 – AI + 3D Hybrid Pipeline

## Goal

3D 모델링 입력 데이터를 AI와 연동하여 하이브리드 제작

## Techniques

- Depth map 연동
- Normal map 활용
- 3D Mesh → 이미지 합성
- AI 배경 생성 + 실사 합성

## Pipeline Flow

Pre-production
→ 3D 모델링
→ Depth 추출
→ ComfyUI 생성
→ 영상 합성
→ 업스케일
→ 사운드 & 립싱크

---

# 📊 Efficiency Analysis

| Stage | 기존 작업 | AI 도입 후 |
|--------|-----------|------------|
| 콘셉트 시안 제작 | 3~4시간 | 40분 |
| 키비주얼 제작 | 2시간 | 25분 |
| 배경 합성 | 1.5시간 | 20분 |

---

# 🔧 Custom Node & Tool Integration

- Light Control
- Inpainting Advanced
- Upscale + Enhance
- Frame Interpolation
- Lip Sync Node

---

# 💡 Design Philosophy

AI는 결과물이 아니라 “제작 속도와 반복 실험”을 가속하는 도구.

중요한 것은:

- 파이프라인 설계
- 실패 케이스 분석
- 제작 적용 가능성

---

# 🚀 Future Expansion

- LoRA 학습 기반 전용 캐릭터 제작
- 게임 엔진 연동 (Unreal / Unity)
- 자동 배치 렌더링 시스템 구축
