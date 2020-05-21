git 기본적인 commit, pull, push 는 알거라 생각합니다



이제 이런 상황이 생길 수 있습니다

* 로컬 서버에서 파일을 바꿔서 git이 꼬였다
* 그냥 뭔가 로컬이랑 깃허브랑 다른데 push 하고 싶다



```
sudo git push origin master --force 
```

강제로 push 합니다



근데 pull 할때는 좀 골떄리는게

```
sudo git stash

sudo git pull origin master
```

해야합니다



그런데 commit  message 쓰라면서



> Please enter a commit message to explain why this merge is necessary,
> especially if it merges an updated upstream into a topic branch.

이렇다면



1. press "i"
2. write your merge message
3. press "esc"
4. write ":wq"
5. then press enter



이렇게 하시면 되는거에요\





이상.

