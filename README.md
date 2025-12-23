# 🚩 Python Minesweeper (지뢰찾기) Project

Python과 Pygame 라이브러리를 활용하여 구현한 지뢰찾기 게임입니다. 기본적인 지뢰찾기 로직에 더해 힌트 기능, 난이도 조절, 하이 스코어 저장, 숫자 색 표기 기능, 타이머 표시 기능등 편의 기능을 추가했습니다.

## 🛠️ 개발 환경 및 실행 방법

* **언어:** Python 3.x
* **라이브러리:** Pygame
* **실행 방법:**
    ```bash
    pip install pygame
    python run.py
    ```

---

## ✨ 주요 기능 및 이슈(Issue) 설명

프로젝트 진행 중 해결한 주요 이슈와 구현된 기능들은 다음과 같습니다.

### 1. 숫자 색 표시 기능 (Issue #1)
* **설명:** 숫자에 색을 조금 더 보기 편하게 수정했습니다.
* **스크린샷:**
    ![난이도 조절](<img width="935" height="953" alt="image" src="https://github.com/user-attachments/assets/116c25c9-59a6-4669-9a08-910e9998b5c4" />

)
  
### 2. 난이도 조절 기능 (Issue #2)
* **설명:** 사용자 실력에 맞춰 초급(Beg), 중급(Int), 상급(Adv)으로 난이도를 변경할 수 있습니다.
* **사용법:**  키보드 숫자키 `1`, `2`, `3`을 눌러 변경 가능합니다.
* **스크린샷:**

    ![난이도 조절](<img width="542" height="648" alt="image" src="https://github.com/user-attachments/assets/c48d7c6c-6948-4a0c-a56c-ca3ee625d474" />



) <img width="773" height="881" alt="image" src="https://github.com/user-attachments/assets/36399c22-c26d-4ab5-a1ba-1ea20b47df03" /> <img width="1019" height="1107" alt="image" src="https://github.com/user-attachments/assets/31b04f10-8130-4be9-8ffb-075d9103e7ce" /> 
<img width="1120" height="339" alt="image" src="https://github.com/user-attachments/assets/cc7f42c0-4f6f-4c44-aaab-197f579e4be6" />




### 3. 힌트 기능 (Issue #3)
* **설명:** 게임 진행 중 막혔을 때 안전한 칸 하나를 알려주는 힌트 기능을 구현했습니다.
* **사용법:**  키보드 `H` 키를 입력합니다. 
* **스크린샷:**

    ![힌트 기능](<img width="535" height="602" alt="image" src="https://github.com/user-attachments/assets/6b745848-1dab-4a53-be00-8cedbc588523" />

)

### 4. 하이 스코어(최고 기록) 저장 (Issue #4)
* **설명:** 게임 클리어 시 소요 시간을 기록하고, 로컬 파일(`highscores.txt`)에 저장하여 재실행 시에도 최고 기록(Best Time)을 상단에 표시합니다.
* **스크린샷:**

    ![하이 스코어](<img width="532" height="596" alt="image" src="https://github.com/user-attachments/assets/07d8bb14-e70c-4a29-9086-7197ffb9ba49" />

)

### 5. 타이머 시각적 알림 (Issue #5)
* **설명:** 게임 시간이 60초를 경과하면 타이머의 글자 색상이 **빨간색**으로 변경되어 사용자에게 긴박감을 줍니다. 또한 999초가 넘어가면 타이머가 멈추고 예외처리 됩니다.
* **스크린샷:**

    ![타이머 기능]( <img width="526" height="639" alt="image" src="https://github.com/user-attachments/assets/5d2f470f-a7fa-4c94-b520-be1d98a871fb" />

)


## 📂 프로젝트 구조
```text
📦 Minesweeper-Project
 ┣ 📜 run.py           # 게임 실행 메인 파일 (UI, 입력 처리)
 ┣ 📜 components.py    # 핵심 게임 로직 (지뢰 배치, 보드 상태 관리)
 ┣ 📜 config.py        # 게임 설정 (색상, 화면 크기, 난이도 상수)
 ┣ 📜 highscores.txt   # 최고 기록 데이터 저장 파일 (자동 생성)
 ┗ 📜 README.md        # 프로젝트 기능 설명 및 스크린샷
