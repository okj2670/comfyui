# comfyui
# AI Visual Production Lab
### ComfyUI 기반 이미지·영상·3D 통합 제작 연구

---

## Overview

본 프로젝트는 콜로소 <제너럴리스트로 거듭나는 ComfyUI 올인원 활용백서> 과정을 기반으로,
AI를 활용한 시각 제작 파이프라인을 실험하고 재구성한 포트폴리오입니다.

단순 이미지 생성이 아니라,

“AI를 제작 프로세스에 어떻게 통합할 것인가?”

를 중심으로 설계되었습니다.

---

#  Project 01 – Visual Consistency System

## Problem

- 동일 인물/제품의 반복 생성 시 일관성 붕괴
- 조명 및 구도 변경 시 디테일 손실

## Applied Techniques

- IP-Adapter
- Pose / Depth ControlNet
- Light ControlNet
- Negative Prompt 구조 설계
- Seed 전략 최적화

## Result

- 구도 변경 자동화 가능
- 인물 유지력 향상
- 연출 실험 속도 3배 개선

---

#  Project 02 – Image to Video Pipeline

## Goal

정적 이미지를 영상으로 확장하는 자동화 워크플로우 설계

## Applied

- T2V / I2V 노드 구조
- Wan 2.2 모델 활용
- 프레임 기반 생성
- 업스케일 & 프레임 보간

## Research Focus

- 프레임 일관성 유지
- 모델별 결과 비교
- 렌더링 시간 대비 품질 분석

---

#  Project 03 – AI + 3D Hybrid Workflow

## Goal

3D 입력 데이터를 AI 이미지/영상 생성에 통합

## Techniques

- Depth Map 추출 및 연동
- Normal Map 기반 조명 반영
- AI 배경 생성 + 합성
- 영상 푸티지와 실사 합성

## Pipeline

Pre-Production  
→ 3D Asset 제작  
→ Depth 추출  
→ ComfyUI 생성  
→ 합성  
→ 업스케일  
→ 사운드 & 립싱크

---

#  Efficiency Study

| 작업 | 기존 방식 | AI 통합 후 |
|------|-----------|------------|
| 콘셉트 제작 | 2~3시간 | 30~40분 |
| 배경 합성 | 1.5시간 | 20분 |
| 영상 테스트 컷 | 4시간 | 1시간 |

---

#  Technical Stack

- SDXL
- ControlNet (Canny, Depth, Pose, Light, Tile)
- IP-Adapter
- Wan 2.2
- Inpainting / Outpainting
- Upscale / Frame Interpolation
- Lip Sync

---

#  Design Philosophy

AI는 결과물을 대신 만드는 도구가 아니라,

“반복 실험과 제작 속도를 가속하는 시스템”

이라고 생각합니다.

본 저장소는 결과 이미지보다
파이프라인 구조와 실험 기록에 초점을 둡니다.

---

# Future Work

- 자동 배치 렌더링 시스템
- 3D 엔진 연동
- AI 기반 프리프로덕션 자동화
