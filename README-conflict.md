# 충돌을 내자

- booldook:: 1번
- 충돌 테스트 중입니다.

## 충돌이 나면 아래와 같이 해결한다.

```bash
# origin 최신형상을 local로 가져온다.
git fetch origin

# dev로 checkout한다 -> dev와 feature/booldook merge하는 과정에서 충돌을 해결할 수 있다.
git checkout dev

# origin dev -> local dev pull한다.
git pull origin dev

# 내 local feature/booldook으로 이동한다.
git checkout feature/booldook

# dev에 병합을 시도한다(local에서)
git merge dev

# 충돌이 발생하고, 수신으로 해결한다.
# 이후에 UI에서 commit/push -> github에서 pr을 진행한다.
```
