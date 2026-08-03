# Prism: REFA Core Engine
> **Deterministic Real-time Signal Purification & Extended Information Filtering Framework**

[![License: Proprietary](https://img.shields.io/badge/License-All%20Rights%20Reserved-red.svg)]()
[![Patent Status](https://img.shields.io/badge/Patent-Pending-orange.svg)]()
[![Python Version](https://img.shields.io/badge/python-3.10%2B-blue)](https://www.python.org/)

---

## 🚀 Overview
**Prism**은 전자전(EW) 및 극한의 노이즈 환경에서 적군의 DRFM(디지털 무선주파수 메모리) 기만 재밍을 실시간으로 차단·격리하고, 정보 행렬 대수적 갱신을 통해 비선형 상태 추정 오차를 수학적 물리 한계선인 **크래머-라오 하한(CRB)**까지 수렴시키는 고성능 소프트웨어 알고리즘 코어입니다.

---

## 📊 Benchmark & Performance Report
아래 벤치마크 결과는 DRFM 기만 재밍으로 오염된 복합 시계열 신호(Composite Stream)에서 REFA 알고리즘이 고에너지 극값을 실시간 격리하고, 0.09ms 대의 결정론적 연산 지연 시간(Steady-State Execution Latency)을 달성함을 증명합니다.

![Prism Benchmark Report](assets/poc_benchmark_report.png)

---

## 🛠️ Core Architecture & Key Modules

1. **Rényi Entropy Filtering (REFA)**
   - 차수 극한 설정($\alpha \to \infty$)을 통해 DRFM 재밍으로 인해 발생하는 고에너지 극값(Tail behavior)과 확률 분포 왜곡을 정밀 감지하고 오염된 데이터를 실시간 격리합니다.
2. **Extended Information Filter (EIF)**
   - 공분산 행렬 중심의 역행렬 연산 오류를 배제하고, 정보 행렬 자체의 대수적 덧셈 연산을 통해 비선형 궤적 추정 정확도와 수치 안정성을 극대화합니다.
3. **CRB Convergence Control**
   - 센서의 피셔 정보와 필터 잔차를 모니터링하여 최종 추정 오차가 물리적 최적 하한선인 크래머-라오 하한(CRB)에 밀착 수렴하도록 제어합니다.

---

## 📂 Repository Structure
```text
Prism/
├── assets/
│   └── poc_benchmark_report.png
├── core/
│   ├── refa.py             # Rényi Entropy Filtering Core
│   ├── eif.py              # Extended Information Filter Module
│   └── crb_control.py      # CRB Convergence Control Logic
└── README.md
```

## 📄 독점 및 법적 고지 (Proprietary & Legal Notice)
Copyright © 2026 Landuaer. All rights reserved. 

본 소스 코드, 문서 및 관련 지식재산권(대한민국 특허 출원번호: 10-2026-0143555)은 란더(Landuaer)의 독점 자산이며 기밀 사항입니다. 본 프로젝트의 핵심 로직(Core Logic)은 프라이빗 레포지토리(Private Repository)에서 엄격히 관리되고 있으며, 본 소프트웨어 코어의 무단 복사, 수정, 배포 또는 상업적 이용은 엄격히 금지됩니다.
