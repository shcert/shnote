# SPAN(Switched Port Analyzer)

`네트워크에서 특정 포트의 모든 트래픽을 모니터링하는 기술을 말합니다.` 

SPAN은 네트워크에서 문제가 발생할 때 이를 해결하기 위해 사용되며, 네트워크 장비나 소프트웨어를 이용해 구현할 수 있습니다. SPAN을 이용하면, 네트워크에서 전송되는 모든 데이터를 모니터링할 수 있어서, 문제가 발생한 원인을 파악하고 해결할 수 있습니다.

예를 들어, 네트워크에서 특정한 서비스가 느리게 동작한다면, SPAN을 이용하여 해당 서비스를 제공하는 서버의 포트를 모니터링하면, 해당 서버로 전송되는 모든 패킷을 살펴볼 수 있습니다. 이를 통해 서버에 문제가 있는지, 네트워크에서 문제가 발생한 것인지를 확인할 수 있습니다.

또한, SPAN은 보안 분야에서도 사용됩니다. 네트워크에서 발생하는 모든 트래픽을 모니터링하면, 불법적인 행위나 해킹 시도를 감지할 수 있습니다. 이를 통해 보안 위협에 대한 대응책을 마련할 수 있습니다.

# 장점
* 스위치를 이용하여 간단하게 구현할 수 있어서 비용이 적게 듭니다.
* 네트워크 인터페이스가 필요 없어서 서버의 부하가 적습니다.
* 스위치에서 모니터링을 할 수 있어서 원격에서 쉽게 접근할 수 있습니다.

# 단점
* 모니터링 대상 포트에 부하를 줄 수 있습니다.
* 모니터링 대상 포트의 데이터를 일부만 캡처할 수 있어서 데이터 손실이 발생할 수 있습니다.
* 모니터링 대상 포트와 다른 포트 간의 상호작용을 볼 수 없습니다.