
### `Java 기초 중간 과제` Nhnmart Servlet version 마무리

* 기존 기능 위에다
    * 로그인/로그아웃
    * 상품 목록
    * 장바구니 담기
    * 장바구니 화면
    * 언어 변경
* MVC Pattern + FrontController Pattern 적용 <span style="color:deeppink">**실습 마무리**</span>
    * JSP 내 Scriptlet 사용 최소화
* 결재 기능 추가
    * 로그인하면 사용자에게 돈 20\_000 원 부여 <span style="color:deeppink">**new**</span>
* 초기화면
    * 상품 목록 링크
    * 장바구니 링크
    * 현재 언어(`ko` or `en`) 표시 <span style="color:deeppink">**new**</span>
    * 잔고 (사용자에게 부여된 돈에서 사용하고 남은 금액) 표시 <span style="color:deeppink">**new**</span>
* 장바구니
    * 장바구니 담기
        * 상품 수량 부족 시 `AmountException`
    * 장바구니에 담긴 물건 선택해서 결재: `POST /pay` <span style="color:deeppink">**new**</span>
        * 결재한 금액 표시
        * 결재 후 잔액 표시
        * 잔액 부족 시 `NotEnoughMoneyException`
* 모든 메세지는 영어, 한국어 2개 언어 지원