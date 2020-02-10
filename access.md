# KMLA Online 접근 방법

* SSH Client를 실행합니다.
* SSH Client를 통해 KMLA Online에 접속합니다.
* 이때 포트는 `220`번을 사용합니다. 아래에서 `cho`를 여러분의 `username`으로 바꾸세요.

```zsh
➜ ~ ssh cho@kmlaonlinet.net -p 220
```
> ⚠️ 보안 설정 때문에 The authenticity of host can't be established.라는 메시지가 나올 때가 있는데 수정 바람

* KMLA Online 서버 코드는 `/srv/http/kmla`에 있습니다.
* `git pull`을 하면 자동으로 `git pull origin master`가 됩니다.
* 필요한 경우에만 제한적으로 `sudo` 명령어를 앞에 붙여 사용하면 됩니다.

```zsh
➜ ~ sudo git pull origin master
```