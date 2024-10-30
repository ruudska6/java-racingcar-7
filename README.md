# java-racingcar-precourse

# 프리코스 2주차 과제 : 🏎️ 자동차 경주

> 우아한테크코스 7기 2주차 미션, 자동차 경주를 구현한 저장소입니다.

# 목차

- [시작하기](#시작하기)
- [기능 목록](#기능-목록)
    - [경주 시작](#경주-시작)
    - [경주](#경주)
    - [경주 끝](#경주-끝)

## 시작하기

레포지토리를 Clone 하고 IDE에서 애플리케이션을 실행합니다.

```git
git clone -b as --single-branch https://github.com/ruudska6/java-racingcar-7/tree/ruudska6
```

## 기능 목록

---

## 경주 시작
- [ ] **사용자에게 자동차 이름 입력을 지시하는 메세지 출력**
    -  `경주할 자동차 이름을 입력하세요.(이름은 쉼표(,) 기준으로 구분).` 가 콘솔에 출력됨.
- [ ] **사용자가 자동차 이름들을 입력한다.**
    - 사용자로부터 생성할 자동차 이름들을 콘솔을 통해 입력받는다.
    - 예시: pobi,woni,jun
    - 예외: 자동차 이름은 쉼표(,)를 기준으로 구분하며 이름은 5자 이하만 가능하다.
    - 사용자가 `잘못된 값을 입력할 경우` `IllegalArgumentException`을 발생시킨 후 애플리케이션은 종료되어야 한다.
    - `1대`만 있을 경우 경주를 할 수 없어 종료.
- [ ] **입력받은 이름을 가진 자동차 객체 n대를 생성한다.**

- [ ] **사용자에게 시도할 횟루를 입력을 지시하는 메세지 출력**
  - `시도할 횟수는 몇 회인가요? ` 
- [ ] **사용자가 몇번의 이동(반복)을 할것인지 입력을 받는다.**
  - 예시: 5
  - 예외: 숫자가 아닌 다른 문자나 음수나 0을 입력할 경우 종료
## 경주
- [ ] **무작위 숫자 생성기**
  - `0에서 9` 사이에서 `무작위 값`을 구한다.
- [ ] **주어진 횟수 동안 n대의 자동차 전진 혹은 정지**
    -  무작위 값이 `4` 이상일 경우 `한 칸` 전진. 아니면 `멈춤`.

- [ ] **자동차가 이동한 거리를 `-` 로 나타냄.**
    - 예시: 3칸 이동시   
    pobi : ---

## 경주 끝
- [ ] **최종 우승자를 선정한다.**
    -  가장 많은 거리를 이동한 자동차를 우승 시킨다.
    - 예시 :  
    pobi : -----  
    woni : ----  
    jun : -----    
    - `최종 우승자 : pobi` 출력
    - 예외 : 동일한 점수가 있다면 `전부` 출력
      - 예시 : `최종 우승자 : pobi, jun` 출력
