# 엔토스 PCB 사이트 편집 방법
## 초기 설정
```
gitbook install
```

## 편집
pcb repository 의 폴더 구조와 동일하게 폴더 및 제품명 사용하여 markdown 문서 작성

### local Test
```
gitbook serve
```

## Publish
편집 완료 후 사이트로 올리기
```
$ gitbook build
$ git checkout gh-pages
$ git pull origin gh-pages
$ xcopy .\_book\* %cd% /y /s /e
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
