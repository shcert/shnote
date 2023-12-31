# MAC(Message Access Code)
메시지 인증 코드(MAC)는 메시지의 무결성과 인증을 보장하는 암호화 기술입니다. MAC는 메시지와 함께 전송되는 인증 코드이며, 이 코드를 통해 수신자는 메시지가 송신자에 의해 생성되었음을 확인하고, 메시지가 전송 도중 변조되지 않았음을 보장할 수 있습니다.

MAC의 구조는 대칭키 암호화 방식과 유사합니다. 송신자는 메시지를 암호화하는데 사용할 비밀키를 생성하고, 이 비밀키를 사용하여 메시지와 함께 MAC를 생성합니다. 수신자는 이 비밀키를 사용하여 메시지를 복호화하고, 송신자가 생성한 MAC와 수신한 MAC를 비교하여 메시지의 무결성과 인증을 확인합니다.

MAC는 다양한 암호화 알고리즘을 사용하여 생성될 수 있습니다. 대표적인 MAC 알고리즘으로는 HMAC, CMAC, GMAC 등이 있습니다. 이 알고리즘들은 안전하고 효과적인 메시지 인증을 보장하기 위해 해시 함수, 블록 암호화 등 다양한 암호화 기술을 사용합니다.

MAC는 중요한 데이터를 전송하는 데 있어서 매우 중요한 보안 기술입니다. 하지만, MAC는 송신자와 수신자가 비밀키를 공유하고 있어야 하기 때문에, 비밀키의 안전한 공유와 관리가 필수적입니다. 또한, MAC를 사용할 때는 적절한 암호화 알고리즘과 키 길이를 선택하고, MAC의 사용 방법을 명확히 정의해야 합니다. 이를 위해서는 보안 전문가들이 MAC의 원리와 구조를 잘 이해하고, 적절한 보안 정책을 수립하고 시행하는 것이 필요합니다.

# 특징 
1. 하이브리드 암호체계를 사용한다.
2. 제 3자에 의한 reply를 부인방지할수가 없다(전자서명을 해야한다)
3. 그냥사용하면은 reply attack에 취약하다.
4. 