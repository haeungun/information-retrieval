# Evaluation in IR System
검색 결과의 질을 평가하는 방법


## IR System Evaluation 
테스트 collection 에는 다음 세가지가 필요
1. 문서 collection
2. Query 로 표현 가능한 test information nees sets
3. 각 (document, query) 페어 간의 relevance 정보

### 기본적인 Term
1. **Information Need** : 유저가 알고 싶어하는 정보</br>
  ex) 레드 와인이 화이트 와인을 마시는 것보다 심장병을 예방하는 데에 효과적인가
2. **Query** : Information Need 의 한가지 표현 방식</br>
  ex) 와인 AND 레드 AND 화이트 AND 심장병 AND 효과
3. **Relevance** </br>
  일반적으로 이진(binary) 속성으로 나타내며, 단순히 query term 을 다 포함해야 relevant한 것이 아니라, **Information Need** 를 잘 충족시켜야 relevant 한것
  
> Recall: Relevant 문서 중 검색 된 비율 </br>
> Precision: 검색된 문서 중 relevant 문서의 비율


