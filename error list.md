# 발생한 에러 리스트

from git
```
error src refspec main does not match any
```
깃 리포지토리에 파일을 올릴때 로컬 폴더에 있는내용과 리포지토리에 있는 내용이 다를 때 발생하는 오류 
```
git pull origin main
```
을 사용해 로컬폴더와 리포지토리에 있는 내용을  똑같이 맞춰주면 해결된다
```
git push -f origin main
```
을 사용해 강제로 push 했을경우 리포지토리에 있는파일이 사라질 수있음
