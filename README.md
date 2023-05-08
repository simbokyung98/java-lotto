# 로또
## 진행 방법
* 로또 요구사항을 파악한다.
* 요구사항에 대한 구현을 완료한 후 자신의 github 아이디에 해당하는 브랜치에 Pull Request(이하 PR)를 통해 코드 리뷰 요청을 한다.
* 코드 리뷰 피드백에 대한 개선 작업을 하고 다시 PUSH한다.
* 모든 피드백을 완료하면 다음 단계를 도전하고 앞의 과정을 반복한다.

## 온라인 코드 리뷰 과정
* [텍스트와 이미지로 살펴보는 온라인 코드 리뷰 과정](https://github.com/next-step/nextstep-docs/tree/master/codereview)

## 기능요구사항 : Step1
* 사용자가 입력한 문자열 값에 따라 사칙연산을 수행할 수 있는 계산기를 구현해야 한다.
* 입력 문자열의 숫자와 사칙 연산 사이에는 반드시 빈 공백 문자열이 있다고 가정한다.
* 나눗셈의 경우 결과 값을 정수로 떨어지는 값으로 한정한다.
* 문자열 계산기는 사칙연산의 계산 우선순위가 아닌 입력 값에 따라 계산 순서가 결정된다. 즉, 수학에서는 곱셈, 나눗셈이 덧셈, 뺄셈 보다 먼저 계산해야 하지만 이를 무시한다.
* 예를 들어 2 + 3 * 4 / 2와 같은 문자열을 입력할 경우 2 + 3 * 4 / 2 실행 결과인 10을 출력해야 한

## 기능목록 : Step1
* 덧셈 기능
* 뺄셈 기능
* 곱셈 기능
* 나눗셈 기능
* 사칙 연산을 모두 포함하는 기능 구현
* 입력 값이 null이거나 빈 공백 문자일 경우 IllegalArgumentException throw
* 사칙연산 기호가 아닌 경우 IllegalArgumentException throw

## 기능요구사항 : Step2
* 로또 구입 금액을 입력하면 구입 금액에 해당하는 로또를 발급해야 한다.
* 로또 1장의 가격은 1000원이다.

## 기능목록 : Step2
* 로또 번호는 1~45 범위내에서 중복없는 6개의 숫자로 이루어 진다.
* 로또 티켓은 발행시 자동으로 생성된 로또 번호를 갖는다.
* 로또 티켓은 당첨번호를 받아 자신의 로또 번호와 비교하여 몇개가 일치하는지 반환한다.
* 구매자로부터 구입금액을 입력 받는다.
* 로또 티켓의 1장의 가격은 1000원 이다.
* 로또 발행기는 입력받은 구입금액을 1장당 가격으로 나눈만큼 로또 티켓을 발행한다.
* 로또 추첨기는 당첨번호와 로또 티켓들을 입력받아 당첨 통계 및 수익률을 산출한다.
* 추첨 결과는 화면을 통해 출력한다.