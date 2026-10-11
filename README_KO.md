# Hero Slayer Moves (Fabric 1.20.1)

## 조작법 (딱 5개)
| 키 | 동작 |
|---|---|
| 맨손 + 좌클릭 | 4연타 콤보 모션 (스트레이트 → 스트레이트 → 훅 → 돌려차기) |
| Z | 돌진 일격 (앞으로 돌진하며 펀치) |
| X | 라이징 어퍼 (적을 공중으로 띄움) |
| C | 회전 킥 (주변 전체 공격) |
| V | 난무 (연타 후 마무리 강타) |

키는 설정 > 조작 > "히어로 슬레이어"에서 바꿀 수 있습니다.

## 설치 (플레이만 할 때)
1. Fabric Loader 설치 (마인크래프트 1.20.1)
2. Fabric API 를 mods 폴더에 넣기
3. 빌드된 `heroslayer-1.0.0.jar` 를 mods 폴더에 넣기 -> 끝
   (서버에서 같이 쓰려면 서버와 접속자 모두에게 설치)

## 직접 빌드하기
1. JDK 17 설치
2. IntelliJ IDEA(Community 무료) 설치 -> 이 폴더를 "Open" -> Gradle 동기화 대기
3. 오른쪽 Gradle 탭 > Tasks > build > build 더블클릭
4. `build/libs/heroslayer-1.0.0.jar` 가 완성본
   (터미널: `gradle build` 또는 `gradle wrapper` 후 `./gradlew build`)

## 모션/수치 고치기
- 모션: `client/anim/Animations.java` (각도 숫자만 수정)
- 쿨타임/데미지/판정: `HeroSlayerMod.java`
- 팔이 반대로 휘두르는 등 방향이 이상하면 해당 줄의 부호(+/-)만 바꾸면 됩니다.
