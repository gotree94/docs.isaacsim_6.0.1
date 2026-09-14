# Isaac Sim이란?

---

**1.Getting Started (시작하기)**
**2.Tutorials (튜토리얼)**
**3.Isaac Sim Workflow Overview (Isaac Sim 워크플로 개요)**
**4.Robotics Ecosystem (로봇 생태계)**
**5.Open Source & Community (합성 데이터 생성)**

---

* URDF, MJCF, Onshape CAD 또는 USD에서 로봇과 씬을 가져옵니다. <br>
PhysX 또는 Newton으로 시뮬레이션하고, RTX 및 물리 기반 센서를 추가하며, <br>
합성 데이터를 생성하고, Isaac Lab을 위한 로봇을 준비하고, ROS 2로 로봇 스택을 검증합니다.

* URDF (Unified Robot Description Format)
   * ROS(Robot Operating System)에서 주로 사용하는 XML 기반의 로봇 모델링 규격입니다.
   * 로봇의 링크(Link), 관절(Joint), 시각적/물리적 특성을 정의합니다.

* MJCF (MuJoCo Format)
   * 로봇공학 및 강화학습 시뮬레이터인 MuJoCo에서 사용하는 XML 기반 모델 파일 포맷입니다.
   * 기계적 구동기, 피부, 제어 요소 및 복잡한 물리적 상호작용을 정밀하게 기술하도록 설계되었습니다.

* Onshape CAD (Computer-Aided Design)
   * Onshape는 웹 기반 SaaS CAD 플랫폼이며, 여기서 CAD는 Computer-Aided Design(컴퓨터 지원 설계)의 약자입니다.
   * 컴퓨터를 활용해 2D/3D 기계 부품 및 조립품을 설계하는 기술 전반을 의미합니다.

* USD (Universal Scene Description)
   * 픽사(Pixar)에서 개발한 오픈소스 3D 씬 확장 규격입니다.
   * 엔비디아 Omniverse 등 최신 그래픽스 및 3D 로보틱스 시뮬레이션 환경에서 복합적인 3D 에셋과 라이팅,
   * 물리 속성을 통합 관리하는 표준 프레임워크로 널리 사용됩니다.

---
* [Quick Install](https://docs.isaacsim.omniverse.nvidia.com/6.0.1/installation/quick-install.html)
* [Tutorial](https://docs.isaacsim.omniverse.nvidia.com/6.0.1/#tutorials)
* [GitHub에서 오픈 소스로 공개](https://github.com/isaac-sim)

---

## 시작하기

작업 방식에 맞는 설정을 선택하세요. 대부분의 사용자는 **빠른 설치**로 시작하는 것이 좋습니다. Python이나 컨테이너 방식은 pip, conda, CI 또는 원격 워크플로에 적합합니다.

| 설치 방식 | 설명 |
|-----------|------|
| [**빠른 설치**](https://docs.isaacsim.omniverse.nvidia.com/6.0.1/installation/quick-install.html#isaac-sim-quick-install) | 로컬 환경을 빠르게 설정하는 가장 빠른 경로 |
| [**워크스테이션 설정**](https://docs.isaacsim.omniverse.nvidia.com/6.0.1/installation/install_workstation.html#isaac-sim-app-install-workstation) | 전체 앱과 로컬 의존성 설치 |
| [**컨테이너 설정**](https://docs.isaacsim.omniverse.nvidia.com/6.0.1/installation/install_container.html#isaac-sim-app-install-container) | Docker에서 Isaac Sim을 실행하여 반복 가능한 환경 구성 |
| [**Python 환경**](https://docs.isaacsim.omniverse.nvidia.com/6.0.1/installation/install_python.html#isaac-sim-app-install-python) | pip 또는 conda를 사용한 Python 기반 워크플로 |

> **팁**: 문제가 발생하면 [설정 팁](https://docs.isaacsim.omniverse.nvidia.com/6.0.1/installation/install_faq.html)공통 수정 방법 또는 [문제 해결](https://docs.isaacsim.omniverse.nvidia.com/6.0.1/overview/troubleshooting.html#isaac-sim-troubleshooting) 페이지를 참조하세요.

---

## 튜토리얼

가장 많이 찾는 주제부터 시작하세요: 첫 번째 시뮬레이션, 로봇 가져오기, 센서, ROS 2, 합성 데이터, 로봇 학습 등.

### 초급

앱, 씬, 핵심 로봇 워크플로를 학습합니다.

| 튜토리얼 | 설명 |
|----------|------|
| [**Isaac Sim 기본 사용법**](https://docs.isaacsim.omniverse.nvidia.com/6.0.1/introduction/quickstart_isaacsim.html#isaac-sim-app-intro-quickstart) | UI 탐색, 씬 불러오기, 첫 번째 시뮬레이션 실행 |
| [**Python 스크립팅 입문**](https://docs.isaacsim.omniverse.nvidia.com/6.0.1/python_scripting/index.html#isaac-sim-app-python-scripting-overview) | 로봇과 환경을 제어하는 첫 번째 독립 스크립트 작성 |
| [**URDF 첫 번째 가져오기**](https://docs.isaacsim.omniverse.nvidia.com/6.0.1/importer_exporter/import_urdf.html#isaac-sim-app-tutorial-advanced-import-urdf) | URDF 로봇을 Isaac Sim으로 가져오고, 구성하고, 시뮬레이션 |

### 중급

ROS 2 연결, 시뮬레이션 제어, 데이터 생성 워크플로 구축.

| 튜토리얼 | 설명 |
|----------|------|
| [**ROS 2 TurtleBot 시리즈**](https://docs.isaacsim.omniverse.nvidia.com/6.0.1/ros2_tutorials/tutorial_ros2_turtlebot.html#isaac-sim-app-tutorial-ros2-turtlebot) | TurtleBot의 가져오기부터 주행, 센서, 타이밍, 변환까지 |
| [**Replicator로 합성 데이터 생성**](https://docs.isaacsim.omniverse.nvidia.com/6.0.1/replicator_tutorials/tutorial_replicator_sdg_workflows.html#isaac-sim-app-tutorial-replicator-sdg-workflows) | Replicator로 Isaac Sim 씬에서 레이블이 달린 학습 데이터 생성 |
| [**ROS 2 시뮬레이션 제어**](https://docs.isaacsim.omniverse.nvidia.com/6.0.1/ros2_tutorials/tutorial_ros2_simulation_control.html#isaac-sim-app-tutorial-ros2-simulation-control) | ROS 2 서비스와 액션을 사용하여 월드 로드, 엔티티 생성, 시뮬레이션 단계 제어 |

### 고급

정책 학습, 씬 무작위화, 결과 배포.

| 튜토리얼 | 설명 |
|----------|------|
| [**Isaac Lab을 위한 로봇 준비**](https://docs.isaacsim.omniverse.nvidia.com/6.0.1/isaac_lab_tutorials/index.html#isaac-lab-tutorials-page) | Isaac Sim에서 로봇 리깅 및 씬 설정으로 Isaac Lab 정책 학습 지원 |
| [**AMR 내비게이션 합성 데이터**](https://docs.isaacsim.omniverse.nvidia.com/6.0.1/replicator_tutorials/tutorial_replicator_amr_navigation.html#isaac-sim-app-tutorial-replicator-amr-navigation) | 무작위화된 창고 씬에서 AMR을 주행하고 관심 객체 근처에서 스테레오 카메라 데이터 캡처 |
| [**ROS 2 정책 평가**](https://docs.isaacsim.omniverse.nvidia.com/6.0.1/ros2_tutorials/tutorial_ros2_rl_controller.html#isaac-sim-app-tutorial-ros2-rl-controller) | Isaac Sim이 관측을 제공하고 작업을 수신하는 상태에서 ROS 2를 통한 강화 학습 정책 실행 |

---

## Isaac Sim 워크플로 개요

### 시뮬레이션 개발 루프
  * 에셋을 가져오고, 로봇과 씬을 구성하고, 동작을 시뮬레이션한 다음, 외부 스택을 연결합니다.

### 개요 (Overview)
  * 각 단계는 재사용 가능하게 유지됩니다. 자산 준비, 로봇 및 씬(Scene) 구성, 시뮬레이션, 스택 연결 모두가 공유된 Isaac Sim 씬에서 작동합니다.

### 합성 데이터 생성 (Synthetic Data Generation, SDG)
  * SDG를 위해 씬에 라벨을 지정하고, 조건에 변형을 주며, 동작을 시뮬레이션하고, 다운스트림 데이터셋을 위한 센서 출력을 렌더링합니다.

### 소프트웨어 인 더 루프 테스트 (Software-in-the-loop Testing, SIL)
  * SIL을 위해 로봇 물리 특성, 센서, 통신 그래프를 구성한 후, 실제 하드웨어 적용에 앞서 외부 로봇 스택을 검증합니다.



| 단계 | 설명 |
|------|------|
| **01 - 가져오기** | 씬, 로봇, 센서, 에셋 |
| **02 - 구성** | 공유 설정 및 워크플로별 배선 |
| **03 - 시뮬레이션** | 월드 실행 및 결과 캡처 |
| **04 - 연결/배포** | 학습 파이프라인 또는 로봇 스택으로 결과 전송 |

### 공유 Isaac Sim 씬

USD 씬, 물리 상태, 센서, 의미 체계, 그래프를 하나의 런타임에서 관리.

| 단계 | 설명 |
|------|------|
| **01 - 가져오기** | 로봇, 씬, 센서, CAD, DCC, 재구성 에셋을 공유 USD 워크스페이스로 가져오기 |
| **02 - 구성** | 재료, 센서, 시나리오, 의미 체계, 로봇 물리, 통신 그래프 설정 |
| **03 - 시뮬레이션** | 조립된 씬에서 물리, 센서 출력, Replicator 캡처, 스택 동작 실행 |
| **04 - 연결/배포** | 학습 파이프라인으로 데이터셋 내보내기 또는 외부 로봇 스택 연결 |

---

## 로봇 생태계

NVIDIA 로봇 생태계의 구성 요소와 Isaac Sim이 어디에 적합한지 이해합니다.

### 소프트웨어 인 더 루프(SIL) 테스트

각 행은 워크플로 단계와 이를 지원하는 NVIDIA 구성 요소를 보여줍니다.

| 단계 | 구성 요소 | 설명 |
|------|----------|------|
| **01 - 씬 구축 및 로봇 리깅** | **Isaac Sim** (로봇 시뮬레이터) | USD 씬 조립, 물리 및 센서 실행, 외부 로봇 스택 연결 |
| **02 - RL/IL 정책 학습** | **Isaac Lab** (선택, RL/IL 프레임워크) | 병렬 환경에서 강화 학습 및 모방 학습 정책 학습 |
| **03 - 대규모 정책 평가** | **Lab - Arena** (선택, 정책 벤치마크) | 여러 씬과 시드에서 학습된 정책 벤치마크 및 비교 |
| **04 - 통합 SIL 테스트 실행** | **Isaac Sim** (SIL 테스트 스택) | ROS 2 또는 Isaac ROS 로봇 스택으로 소프트웨어 인 더 루프 테스트 실행 |

---

## 합성 데이터 생성

---

## 오픈 소스 & 커뮤니티

Isaac Sim은 오픈 소스이며 기존 로봇 스택에 맞춰 빌드되었습니다. 제공되는 도구를 사용하고, 코드를 읽고, Python과 Kit로 시뮬레이터를 확장하세요.

| 항목 | 설명 |
|------|------|
| **오픈 소스 플랫폼** | 코드를 읽고, 시뮬레이터를 확장하고, 스택에 맞춤 |
| **Apache 2.0** | 시뮬레이터 스택용 오픈 소스 라이선스 |
| **USD 네이티브** | 에셋 가져오기부터 배포까지 하나의 씬 표현 |
| **PhysX + Newton** | 하나의 시뮬레이터에서 지원되는 물리 백엔드 전환 |
| **RTX + 물리 센서** | 렌더링과 물리 기반 센서 모델을 한 곳에서 사용 |

| 링크 | 설명 |
|------|------|
| **포럼** | NVIDIA 개발자 커뮤니티에서 질문하고 도움 받기 |
| **Discord** | 다른 Isaac Sim 사용자 및 개발자와 실시간 채팅 |
| **출시 노트** | Isaac Sim 릴리스의 최신 기능, 수정 사항, 버전 변경 추적 |
| **도움말 & FAQ** | 일반적인 설치 수정, 문제 해결, 지원 안내 |

---

*이 페이지가 도움이 되었나요?*
