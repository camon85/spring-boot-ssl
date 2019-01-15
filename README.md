# Self-Signed Certificate
로컬 개발 환경에서도 https를 사용하는 방법

# keytool 위치
$JAVA_HOME/bin/keytool

# 인증서 생성
keytool -genkeypair -alias camon -keyalg RSA -keysize 2048 -storetype PKCS12 -keystore camon.p12 -validity 3650

# 실행 예제
keytool -genkeypair -alias camon -keyalg RSA -keysize 2048 -storetype PKCS12 -keystore camon.p12 -validity 3650
키 저장소 비밀번호 입력: 123456
새 비밀번호 다시 입력: 123456
이름과 성을 입력하십시오.
  [Unknown]:  camon
조직 단위 이름을 입력하십시오.
  [Unknown]:  camon
조직 이름을 입력하십시오.
  [Unknown]:  camon
구/군/시 이름을 입력하십시오?
  [Unknown]:
시/도 이름을 입력하십시오.
  [Unknown]:
이 조직의 두 자리 국가 코드를 입력하십시오.
  [Unknown]:  ko
CN=camon, OU=camon, O=camon, L=Unknown, ST=Unknown, C=ko이(가) 맞습니까?
  [아니오]:  y
  
 
 # 테스트 
 <https://localhost:8443/hello>
