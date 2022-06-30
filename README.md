# Git-GitHub-Tutorial-PR
Git&amp;GitHub Tutorial for PR

## Fork Me!
Fork는 아주 큰 협업 프로젝트에 기여할 수 있는 멋진 방법입니다.

만약 이 remote repo를 fork했다면, 당신의 계정에 이와 똑같이 생긴 remote repo가 생성되었을 것입니다.

그렇다면 다음 커맨드를 입력하여 당신의 repo를 local repo로 복제해 오세요:
```
git clone [your repo's link]
```

## Remote Me!
이제 당신이 가지고 있는 local repo는 당신의 remote repo와 연결되어 있을 겁니다.

**다시 말해**, 당신이 local repo를 아무리 수정해봤자 원본 remote repo와는 하등 관계가 없다는 뜻입니다.

정말 당신이 원본 repo에 기여를 하고 싶다면, 원본 repo에 수정사항을 제안(이것이 PR입니다)할 수 있도록 remote repo에 원본 repo를 추가해야 합니다.

다음과 같이 커맨드를 입력하여 추가할 수 있습니다:
```
git remote add [original remote repo's nickname] [original remote repo's link]
```

## Add New Branch!
여러 수정을 거친 후 그에 대한 PR을 안전하게 보내기 위해서는, PR을 위한 branch가 있어야 합니다.

다음의 커맨드를 입력하여 당신의 local repo에 PR용 branch를 만들어 줍시다:
```
git checkout -b [branch name]
```

## And.. You Can Edit This Project As You Wish!
이제 당신은 당신의 local repo가 있는 working directory에서 마음껏 파일을 추가하고, 삭제하고, 수정할 수 있습니다.
바로 해보세요!

원하는 만큼 수정했다면, 마치 개인이 작업했을 때처럼 수정사항을 add하고, commit하고, push할 수 있습니다!
다음의 커맨드를 입력하여 수정사항을 (하고 싶은 만큼) add하고, commit하고, push해봅시다:
```
git add [modified files / if you want to add all of changes, just type -A]
git commit -m "[commit message]"
git push origin [your branch name for PR]
```

## Finally, Create PR!
Push까지 무사히 되었다면, 이제 정말 PR을 날릴 수 있습니다.

지금까지 아무 문제 없이 잘 따라왔다는 전제 하에, 당신의 remote repo 페이지에 새로 push가 되었다며 **Compare $ pull request** 버튼이 활성화되었을 겁니다.

이제 이 버튼을 누르면, PR 제목을 기입할 수 있는 란, remote repo에 적용되어 있지 않은 새 commit 이력들과 함께 해당 commit들에 대해 설명할 수 있는 설명란이 나타납니다.
제목과 설명을 정성껏 작성한 뒤, **Create pull request** 버튼을 클릭하면 원본 remote repo에 새 PR이 생성됩니다!

## Congraturations!
축하드립니다! 당신은 PR을 성공적으로 날렸고, 프로젝트 관리자가 당신의 수정사항을 확인한 후 마음에 든다면 merge하여 당신의 노력이 실제 원본 remote repo에 반영될 것입니다!

이후에는 다음을 위해 당신의 remote repo와 local repo에서 PR용 branch를 삭제해 주면 됩니다:
```
git branch -D [your branch name for PR]
git push origin :[your branch name for PR]
```
