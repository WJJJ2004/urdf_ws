# urdf_ws

## 📦 개요

`urdf_ws`는 [fusion2urdf-ros2](https://github.com/dheena2k2/fusion2urdf-ros2)를 기반으로 개발된 ROS 2용 URDF 패키지입니다.  
Autodesk Fusion 360에서 설계한 로봇 모델을 ROS 2 환경에서 시뮬레이션 및 제어할 수 있도록 변환하여 제공합니다.

---

## 🧰 포함된 패키지

### 1. `robit_humanoid_description`

- **용도**: 보행 강화학습용
- **특징**:
  - 6자유도(6DOF)
  - 오프셋 적용

### 2. `robit_humanoid_offset_22DOF_description`

- **용도**: 2025 IEEE Humanoids loco-mani 및 시뮬레이션 개발용
- **특징**:
  - 22자유도(22DOF)
  - Self-collision escape 기능 개발용
  - 

---

## 🔧 설치 및 사용 방법

```bash
# 작업공간 생성 및 클론
mkdir -p ~/ros2_ws/src
cd ~/ros2_ws/src
git clone https://github.com/WJJJ2004/urdf_ws.git

# 빌드 및 환경 설정
cd ~/ros2_ws
colcon build
source install/setup.bash
