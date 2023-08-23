# 공격 종류

# ​SQL 인젝션(Sql injection)

* 외부에서 SQL 쿼리를 삽입하여 시스템 권한을 획득하거나 데이터를 훔치는 공격기법
* 웹 서비스가 예외적인 문자열을 적절히 필터링 하지 못하는 경우 발생

# XSS(Cross-site Scripting)

* 공격자가 작성한 스크립트가 다른 사용자에게 전달되는 것
* 다른 사용자의 웹 브라우저 안에서 적절한 검증 없이 실행되기 떄문에 사용자의 세션을 탈취하거나 웹 사이트를 변조하고 악의적인 사이트로 사용자를 이동할 수 있다.

# CSRF,XSRF(Cross-site request forgery)

* 불특정 다수를 대상으로 로그인된 사용자가 자신의 의지와는 무관하게 공격자가 의도한 행위를 하게 만드는 공격