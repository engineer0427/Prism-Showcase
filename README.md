# Prism: REFA Core Engine
> **Deterministic Real-time Signal Purification & Extended Information Filtering Framework**

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Python Version](https://img.shields.io/badge/python-3.10%2B-blue)](https://www.python.org/)
[![Patent Status](https://img.shields.io/badge/Patent-Pending-orange.svg)]()

---

## 🚀 Overview
**Prism**은 전자전(EW) 및 극한의 노이즈 환경에서 적군의 DRFM(디지털 무선주파수 메모리) 기만 재밍을 실시간으로 차단·격리하고, 정보 행렬 대수적 갱신을 통해 비선형 상태 추정 오차를 수학적 물리 한계선인 **크래머-라오 하한(CRB)**까지 수렴시키는 고성능 소프트웨어 알고리즘 코어입니다.

### ✨ Key Features
- **Rényi Entropy Filtering (REFA)**: 차수 극한 설정($\alpha \to \infty$)을 통한 고에너지 극값 분석 및 비정상 관측치 실시간 격리
- **Extended Information Filter (EIF)**: 공분산 역행렬 연산 오류를 배제하고 정보 행렬의 대수적 덧셈 연산을 통한 0.09ms 대 초고속 전파
- **Hardware-Agnostic Software Core (Black-box IP)**: 특정 하드웨어에 종속되지 않는 모듈형 라이브러리 구조로 다양한 온보드 시스템에 즉시 통합 가능
