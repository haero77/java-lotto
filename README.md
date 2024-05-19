> [미션 리드미](https://github.com/talmood/private-mission-README/tree/main/%EB%AF%B8%EC%85%98%203%20-%20%EB%A1%9C%EB%98%90)

<!-- TOC -->
* [기능 요구사항](#기능-요구사항)
<!-- TOC -->

# 기능 요구사항

- [x] 로또 구입 금액 입력
  - [x] 안내 문구 출력 (`구입금액을 입력해 주세요.`) 
  - [x] 1,000원 단위로 입력받는다.
- [x] 로또 발행 기능
  - [x] 구입한 금액 만큼 로또를 발행한다.
    - [x] 로또 번호는 1부터 45까지 중 중복되는 수 없이 6자리 숫자이다.
  - [x] 발행된 로또를 출력한다. 
    - [x] 구매한 로또 게임 개수 출력 (`14개를 구매했습니다.`)
    - [x] 구매한 로또 게임 숫자 출력 
- [x] 당첨 숫자 입력 기능
  - [x] 6자리 당첨 번호 입력 기능
    - [x] 당첨 번호는 콤마 `,`로 구분한다.
  - [x] 보너스 볼 입력 기능
    - [x] 보너스 볼은 당첨번호와 중복되어서는 안 된다.
- [x] 로또 결과 출력
  - [x] 등수별 당첨 금액 및 당첨 개수를 출력한다.  
  - [x] 수익률을 출력한다. (소수점 이하 둘째 자리에서 반올림하여 출력)
    - [x] 수익률 = 당첨 금액 / 구입 금액

로또 만들 때 Collections.sort 사용해서 정렬하기

---

입출력 예시

```text
구입금액을 입력해 주세요.
14000
14개를 구매했습니다.
[8, 21, 23, 41, 42, 43]
[3, 5, 11, 16, 32, 38]
[7, 11, 16, 35, 36, 44]
[1, 8, 11, 31, 41, 42]
[13, 14, 16, 38, 42, 45]
[7, 11, 30, 40, 42, 43]
[2, 13, 22, 32, 38, 45]
[23, 25, 33, 36, 39, 41]
[1, 3, 5, 14, 22, 45]
[5, 9, 38, 41, 43, 44]
[2, 8, 9, 18, 19, 21]
[13, 14, 18, 21, 23, 35]
[17, 21, 29, 37, 42, 45]
[3, 8, 27, 30, 35, 44]

지난 주 당첨 번호를 입력해 주세요.
1, 2, 3, 4, 5, 6
보너스 볼을 입력해 주세요.
7

당첨 통계
---------
3개 일치 (5000원)- 1개
4개 일치 (50000원)- 0개
5개 일치 (1500000원)- 0개
5개 일치, 보너스 볼 일치(30000000원) - 0개
6개 일치 (2000000000원)- 0개
총 수익률은 0.35입니다.(기준이 1이기 때문에 결과적으로 손해라는 의미임)
```