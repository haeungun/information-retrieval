# Search Engine
검색엔진이 하는 일은 다음과 같다.
1. 인터넷 상의 수많은 문서들을 수집해야 하고(크롤링)
2. 수집한 데이터를 검색엔진이 사용하기 쉽게끔 정리 및 분류하여 검색엔진 데이터베이스에 저장(색인, 인덱싱)하여
3. 사용자가 검색어를 입력했을 때 색인해둔 데이터를 사용해 입력된 검색어에 가장 적합한 문서들을 사용자에게 가져다준다(검색 키워드 처리).

## Web Crawling
검색엔진을 지원하기 위해 웹으로부터 웹 페이지들을 수지하여 색인하는 절차
> 누가 더 많이 수집하고 누가 더 빨리 처리해서 색인기에 집어 넣느냐는 절대적인 성능의 지표

### The costs of using Web crawlers
- 네트워크 리소스: 크롤러는 상당한 대역폭을 필요로 하고 오랜 시간 동안 높은 수준의 병렬 처리로 동작
- 서버 과부하: 특히 지정된 서버에 대해 접근 빈도가 너무 높을 경우
- 잘못 작성된 크롤러: 서버 or 라우터를 크래시하거나 처리할 수 없는 페이지를 다운로드
- 개인 크롤러: 너무 많은 사용자들로부터 배포될 경우, 네트워크 및 웹 서버를 손상시킬 수 있음