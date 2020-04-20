# 여기는 NLP에 대해서 공부한 것들, 구현해본 것들을 모아놓은 폴더입니다~~

# 에러들 모음

## Mecab-user-dic 사용자 사전 추가 [Error 2] 해결하는 방법!!!
- 우선 Mecab-ko, Mecab-ko-dic 차근차근 다 설치하기
- Mecab-ko-dic 디렉토리에서 
  - $ ./autogen.sh
  - $ make
- coreutils 설치하기 
  - $ brew install coreutils
- add-userdic.sh 4번째 줄에서 readlink => greadlink로 바꿔주기!
- 그리고 
  - $ ./tools/add-userdic.sh
- $ make install 하면 끝!

## Rake 라이브러리 nltk가 안 돌아가는 에러 해결하는 방법!!
- nltk.download( ) 이 코드를 돌려준다!
- nltk.download( )에서 'SSL: certificate verify failed' 에러가 뜬가면?
  - python 3.8 폴더에 간다.
  - $ install Certificates.command 코드를 실행시킨다.
  - 그 다음에 다시 nltk.download( )를 실행시켜주면 된다!
