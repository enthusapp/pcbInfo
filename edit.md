# 엔토스 PCB 사이트 편집 방법

## 편집

### 그림 올리기
그림 파일을 프로젝트 폴더에 복사하고 문서에 경로 링크를 추가
```
![그림 설명](그림파일 상대경로)
```

##### 예시
`img` 폴더에 `test.png` 파일이 있을 경우,
```
![테스트 이미지](img/test.png)
```

### local Test
```
gitbook serve
```

## Publish
편집 완료 후 사이트로 올리기
```
$ gitbook build
$ git checkout gh-pages
$ cp -R ../_book/* . // Windows 환경에서는 파일 브라우져에서 덮어쓰기 사용
$ git clean -fx _book
$ git add .
$ git commit -sm "upload gh-pages"
$ git push origin gh-pages
$ git checkout master
```

## PDF 제작
* https://calibre-ebook.com 설치후 명령어 실행
```
gitbook pdf
```
