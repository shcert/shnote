# 서비스 서부공격(Dos) 정리

TCP Syn flooding Attack

    TCP 연결 설정 과정 중에 3-Way Handshaking 과정에서 Half-Open 연결 시도가 가능하다는 취약점을 이용한 공격

Land Attack

     패킷을 전송할 때 송신과 수신 IP주소를 모두 공격대상 IP주소로 하여 데이터를 전송하는 공격기법. 공격대상은 자신에게 무한히 응답하된다.

Teardrop Attack

    오프셋 값을 단편화 간에 중복되도록 고의적으로 수정하거나 정상적인 오프셋 값보다 더 큰 값을 더해 그 범위를 넘어서는 오버플로우를 일으켜 시스템의 기능을 마비시키는 Dos 기법

ping of death

    핑을 이용하여 ICMP 패킷을 정상적인 크기(65,535 bytes)보다 아주 크게 만드는 공격

smurfing Attack
    
    icmp echo를 생성하여 엄청난 양의 데이터를 한 사이트에 집중적으로 보냄으로써 네트워크를 불능 상태로 만드는 공격 방법.

Bonk

    패킷을 프래그먼트하여 전송할 때 패킷을 조작하여 결과적으로 공격대상자에게 시스템 부하를 증가시키는 공격

Boink 

    Bonk를 수정한 Dos 공격도구로서 패킷 시컨스 번호를 비정상적인 상태로 보내는 공격 기술


# jamming형 공격

1. switch 재밍
switch허브의 취약점을 활용한 공격으로 mac주소를 지속적으로 보내어 mac table을 가득채워서 switch허브를 hub로 장비를 부하시켜서 만들어버리는 디도스 공격입니다.  
2. 