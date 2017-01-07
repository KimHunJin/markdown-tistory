# 마크다운으로 작성한 내용을 티스토리로 전송하기

![티스토리](./images/티스토리.png)

![티스토리](./images/티스토리2.png)

![티스토리](./images/티스토리3.png)

### 2017-01-04 진행 상황
* access token 발급 가능
* access token으로 티스토리에 글 게시 가능
* 마크다운 텍스트 HTML로 전환
* 디렉토리+파일명으로 되어있는 문자열 추출해서 파일명만 남기기 가능

### 2017-01-05 진행 상황
* 실행한 디렉토리 내에 있는 마크다운 파일 인식하기
* 해당 마크다운 파일 이름을 게시글 타이틀로 지정하기

### 2017-01-07 진행 상황
* 마크다운 텍스트에 포함된 이미지 파일명만 추출

### 예정
글로벌 설치 방식으로 변경해야 어디서든 마크다운 파일 위치에서 바로 업로드가 가능해서 해당 방식으로 할 예정

* 글로벌 모듈 설치 방식으로 변경 
 
* 마크다운 텍스트에 포함된 이미지 파일 티스토리에 업로드
  - 마크다운 텍스트에 포함된 이미지 파일들 추출하여 multi part data 형태로 티스토리에 전송
  - 전송하여 나온 결과 (즉, 티스토리에 저장된 이미지의 이름)을 마크다운 텍스트의 기존 이미지 코드와 교체

### 참고
* [티스토리 API](http://www.tistory.com/guide/api/post)
* [Nodejs Path 가이드](https://nodejs.org/api/path.html#path_windows_vs_posix)
* [Node form-data](https://github.com/form-data/form-data)
* [Global Module 생성](https://bretkikehara.wordpress.com/2013/05/02/nodejs-creating-your-first-global-module/)