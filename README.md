# Question Answering & Question Generation & answer extration K2-T5 with KorQuAD
학습된 K2-T5 모델을 기반으로 질의응답, 질문 생성, 정답 생성 모델을 만들었습니다. 멀티테스크 모델을 학습시키기 위해 Question Answering 데이터셋인 KorQuAD v1.0을 사용하였습니다.

# 사용 방법
과거 했던 프로젝트 재현을 위해 google colaboratory에서 돌아갈 수 있게끔 코드를 작성하였습니다.
GPU와 큰 메모리를 활성화 시킨 후 모두 실행하시면 됩니다.

## data
- KorQuAD v1.0
- qg,qa,ans_ext 포맷으로 문제를 각각 변경
- QA
  - src : \[\"question: What is the answer to life? context: 42 is the answer tolife, the universe and everything<EOS>\"\]
  - tgt : 42
- QG
  - src : \[\"generate question. answer : 42 context: 42 is the answer to life, the universe and everything.<EOS>\"\]
  - tgt : What is the answer to life?
- ans_ext
  - src : \[\"extract answer. context: 42 is the answer to life, the universe and everything.<EOS>\"\]
  - tgt : 42

## model
- KETI-AIR/ke-t5-small-ko from HuggingFace
- pytorch-lightning
## train
- 
## validation


@ke-T5
