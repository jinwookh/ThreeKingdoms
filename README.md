# ThreeKingdoms
안녕하세요, 삼국지 텍스트를 기초로 프로젝트를 하려고 합니다.

삼국지 텍스트 url: https://ebooks.adelaide.edu.au/l/literature/chinese/romance-of-the-three-kingdoms/

장기적인 관점에서 세 개의 프로젝트를 step by step으로 진행할 것입니다.



## step 1: 삼국지 텍스트 데이터를 기초로 장수 검색엔진 개발 

 * 관련 시나리오: 백엔트 시나리오 3

 * 기능: 장수 이름을 질의하면 장수 이름이 들어간 문장들을 반환한다.

 * 사용기술: elsaticSearch, flask or react(front end), django or node.js (backend)

## step 2: 삼국지 텍스트를 mongoDB에 저장, DB 구조 설정 

 * 관련 시나리오: 데이터 엔지니어링 시나리오 1

 * DB 필드: 'title', 'content', 'chapter', 'characters'

   chapter is the primary key
 * issue: 'characters' field를 입력을 자동화할 수 있는 방법은? 다시 말해, 하나의 chapter에서 인물 이름만 자동으로 뽑을 수 있는 방법이 있는가?
 
 
## step 3 : step 2에서 만든 db를 기반으로, 장수들의 strong set을 만드는 알고리즘 개발

 * apriori 알고리즘을 기반으로 장수들과 강한 연관성을 지닌 단어들을 추출
 
 * key: 장수이름, value: 연관성 있는 단어들인 또다른 db 구성
 
 * 기능: 사용자가 장수이름을 입력하면, 장수와 관계된 단어들을 리턴한다.
 
 * 기술: mongoDB, elasticSearch, flask or react(front end), django or node.js (backend)


