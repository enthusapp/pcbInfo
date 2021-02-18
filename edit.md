# 엔토스 PCB 사이트 편집 방법
## 초기 설정
```
gitbook install
```

### graceful-fs error 수정
https://stackoverflow.com/questions/64211386/gitbook-cli-install-error-typeerror-cb-apply-is-not-a-function-inside-graceful

## 편집
pcb repository 의 폴더 구조와 동일하게 폴더 및 제품명을 사용하여 markdown 문서를 작성합니다.
각 폴더에는 별도의 `README.md` 파일을 생성합니다.
[SUMMARY.md](SUMMARY.md) 에는 새로 생성한 제품에 대한 경로를 추가합니다.

##### 예시
```markdown
# Summary

* [소개](README.md)
* [투광등](flood/README.md)
  * [LFR](flood/lfr/README.md)
    * [LFR0655](flood/lfr/lfr0655/README.md)
      * [LFR0655-120FWC](flood/lfr/lfr0655/lfr0655-120fwc.md)
  * [LFC](flood/lfc/README.md)
    * [LFC0165](flood/lfc/lfc0165/README.md)
      * [LFC0165-48FWC](flood/lfc/lfc0165/lfc0165-48fwc.md)
```

### local Test
```
gitbook serve
```

## Publish
편집 완료 후 사이트로 배포합니다.

1. markdown 변경 사항은 VSCode 를 통해 `master branch` 에 commit 및 push 합니다.
1. 아래 명령을 차례로 입력하여 gitbook 빌드 결과를 gh-pages branch 에 업로드 합니다.

```
gitbook build
git checkout gh-pages
git pull origin gh-pages
xcopy .\_book\* . /y /s /e // windows cmd 는 xcopy .\_book\* %cd% /y /s /e
git clean -fx _book
git add .
git commit -sm "upload gh-pages"
git push origin gh-pages
git checkout master
```

## PDF 제작
* https://calibre-ebook.com 설치후 명령어 실행
```
gitbook pdf
```
