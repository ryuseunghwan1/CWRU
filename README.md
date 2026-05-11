# CWRU Bearing Fault Diagnosis

시계열 인코딩 기법과 딥러닝 모델 구조 간 친화성이 회전기기 결함 진단 성능에 미치는 영향 분석

## 연구 개요

CWRU 베어링 데이터셋을 활용하여 GAF·MTF·RP 인코딩과 ResNet-18·ViT 모델 조합의 성능을 비교 분석한 연구입니다.

## 실험 결과

| 인코딩 | 모델 | 테스트 정확도 |
|--------|------|--------------|
| MTF | ResNet-18 | **99.47%** |
| RP | ViT | 99.34% |
| RP | ResNet-18 | 98.68% |
| GAF | ResNet-18 | 91.94% |
| MTF | ViT | 88.64% |
| GAF | ViT | 64.86% |

## 환경 설정

\`\`\`bash
conda create -n bearing python=3.10
conda activate bearing
pip install -r requirements.txt
\`\`\`

## 데이터셋

CWRU Bearing Data Center에서 다음 파일들을 다운로드하여 프로젝트 루트에 배치:
- \`normal/\` : 97, 98, 99, 100
- \`12k_Drive_End_Bearing_Fault_Data/IR/\` : 105, 106, 107, 108
- \`12k_Drive_End_Bearing_Fault_Data/B/\` : 118, 119, 120, 121
- \`12k_Drive_End_Bearing_Fault_Data/OR/\` : 130, 131, 132, 133

## 저자

- 류승환 (인하대학교 공학대학원 AI융합전공)
- 박주혜 (롯데이노베이트 AI 기술팀)
