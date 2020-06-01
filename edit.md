# 엔토스 PCB 사이트 편집 방법

## 편집

### local Test
```
gitbook serve
```

## Publish
편집 완료 후 사이트로 올리기

```
$ git checkout gh-pages // gh-pages branch 가 없을 경우 git checkout -b gh-pages
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
