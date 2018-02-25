# Shingling
웹은 특징상 다수의 동일한 콘텐츠를 가진다. 따라서 웹 문서의 중복을 감지할 수 있는 방법이 필요하다.
> 웹 상의 40% 정도가 다른 페이지와 중복된다.

## Fingerprint
중복을 감지할 수 있는 가장 간단한 방법이다. 해당페이지에 대한 문자들을 간결하게 압축한 것을 계산하는 것이다.</br>
그러나 near duplication 문제를 해결할 수 없다.

## Shingling
Shingling 은 각 문서를 k 개의 연속된 단어 시퀀스의 집합으로 표현한다. 이러한 집합을 k-shingling 이라고 한다.</br>
Shingling 을 활용한 near duplication 문제 해결은 다음과 같은 과정으로 진행된다.

1. document 에 대해 각 토큰을 분리한다.
2. k-shingling 을 생성한다.
3. 중복 슁글을 제거한다.
4. 최종결과

## Jaccard Similarity
두 document 에 대해 생성된 shingling 집합 간에 유사도를 측정하기 위해 Jaccard 계수를 사용할 수 있다.</br>
두 집합 A, B 에서 Jaccard 계수는 **A, B 교집합의 크기/두 집합의 합 집합의 크기** 로 구할 수 있다.

## Pros and Cons
- 단어의 출현순서가 고려된다. 
- 슁글 크기에 따른 연산 속도와 정확도 사이에 trade-off 존재
> 슁글의 크기가 크다면 연산 비용은 줄어들지만, 그만큼 정확도는 떨어진다. 
