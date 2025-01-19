# Comment_classification_and_generation

이 레포지토리는 혐오 발언 분류 및 생성 작업을 위한 Jupyter Notebook과 관련 리소스를 포함하고 있습니다. 이 프로젝트는 텍스트 데이터에서 혐오 발언을 탐지하고, 생성하며, 평가하는 방법을 탐구하는 것을 목표로 합니다.

## 목차
- [프로젝트 개요](#프로젝트-개요)
- [레포지토리 파일 설명](#레포지토리-파일-설명)
- [설치 및 환경 설정](#설치-및-환경-설정)
- [사용법](#사용법)
---

## 프로젝트 개요
이 프로젝트는 세 가지 주요 구성 요소로 나뉩니다:
1. **혐오 발언 분류**: 주어진 텍스트가 혐오 발언인지 여부를 식별합니다.
2. **혐오 발언 생성**: 특정 속성에 따라 혐오 발언을 생성하여 혐오 언어의 패턴을 이해합니다.
3. **평가**: 분류기와 생성된 텍스트의 성능을 평가합니다.

이 프로젝트는 혐오 발언에 맞서기 위한 연구에 기여하고, 혐오 발언 탐지 방법을 개선하는 것을 목표로 합니다.

---

## 레포지토리 파일 설명

### 1. `hate_comments_classification.ipynb`
이 노트북은 혐오 발언을 분류하는 모델을 학습시키고 평가하는 코드를 포함하고 있습니다. 라벨링된 데이터셋을 사용하며, F1-스코어, 정밀도, 재현율 등의 지표를 통해 성능을 평가합니다.

### 2. `conditional_hate_generation.ipynb`
이 노트북은 혐오 발언인지 아닌지의 조건이 주어진 상태에서 혐오 발언을 생성합니다. 연구 목적으로 혐오 발언 생성을 시뮬레이션하며, 오용 방지를 위한 안전 장치를 구현합니다.

### 3. `evaluate.ipynb`
이 노트북은 분류기 및 생성된 텍스트의 품질과 신뢰성을 평가하기 위한 도구와 방법론을 제공합니다. 평가 지표에는 perplexity, 다양성, 조건과의 의미적 정렬 등이 포함됩니다.

### 4. `hate_generation.ipynb`
이 노트북은 조건 없이 혐오 발언을 생성하는 실험을 다룹니다. 언어 모델을 활용하여 분석 및 연구를 위한 합성 혐오 발언 예제를 생성합니다.

### 5. `normal_generation.ipynb`
이 노트북은 비교 분석을 위해 비혐오(중립) 발언을 생성합니다. 이를 통해 혐오와 중립 발언 간의 언어적, 구조적 차이를 연구합니다.

---

## 설치 및 환경 설정

### 요구 사항
- Python 3.8 이상
- Jupyter Notebook 또는 Jupyter Lab
- 필요한 Python 라이브러리(`requirements.txt`에 명시됨)

### 설치 단계
1. 레포지토리 클론:
   ```bash
   git clone https://github.com/your-username/hate-speech-classification-generation.git
   cd hate-speech-classification-generation
   ```
2. 의존성 설치:
   ```bash
   pip install -r requirements.txt
   ```
3. Jupyter Notebook 실행:
   ```bash
   jupyter notebook
   ```

---

## 사용법

1. **혐오 발언 분류**:
   - `hate_comments_classification.ipynb`를 엽니다.
   - 데이터셋을 로드하고, 모델을 학습시키며, 성능을 평가하는 단계를 따릅니다.

2. **혐오 발언 생성**:
   - 조건부 생성을 위해 `conditional_hate_generation.ipynb`를 사용합니다.
   - 비조건부 생성을 위해 `hate_generation.ipynb`를 사용합니다.

3. **평가**:
   - `evaluate.ipynb`를 열어 분류기와 생성된 텍스트의 성능을 평가합니다.

4. **중립 텍스트 생성**:
   - `normal_generation.ipynb`를 사용하여 중립 텍스트 샘플을 생성합니다.

---

