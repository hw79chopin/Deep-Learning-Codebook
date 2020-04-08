This is repo about NLP

# Mecab-user-dic error 해결하는 방법!!!
- 우선 차근차근 다 설치하기
- Mecab-ko-dic 에서 ./autogen.sh => make를 설치하기
- coreutils를 brew로 설치하기
- add-userdic.sh 4번째 줄에서 readlink => greadlink로 바꿔주기!
- 그리고 ./tools/add-userdic.sh 하고
- make  install로 한다.

## mecab-user-dic과 mecab-ko 폴더의 위치는 mecab이 깔려있는 디렉토리 (e.g 라이브러리)에 놔주면 jupyter notebook에서도 사용가능하다!
