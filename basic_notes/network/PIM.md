# PIM(Protocol Independent Multicast)  

PIM(Protocol Independent Multicast)은 멀티캐스트 데이터를 전송하기 위한 프로토콜 중 하나로, 라우팅 프로토콜과 함께 동작하여 멀티캐스트 데이터를 전송할 수 있는 경로를 생성하고 유지합니다. PIM은 프로토콜에 독립적이므로, 다양한 라우팅 프로토콜과 함께 사용될 수 있습니다.

PIM 프로토콜은 라우터들 간에 멀티캐스트 트래픽을 라우팅하기 위해 사용됩니다. PIM은 다음과 같은 특징을 가집니다.

* 트리 기반 멀티캐스트: PIM은 라우터들 간에 트리 기반 멀티캐스트를 구성합니다. 라우터들은 멀티캐스트 그룹에 가입하여 멀티캐스트 데이터를 수신하고, 멀티캐스트 데이터를 전송하고자 하는 경우에는 멀티캐스트 트리 상에 있는 해당 그룹에 데이터를 전송합니다.
* 자원 절약: PIM은 데이터가 전송되는 경로를 최소화하여 네트워크 자원을 절약합니다. 멀티캐스트 그룹에 대한 경로를 생성하고, 이 경로를 유지하기 위해 라우팅 프로토콜과 함께 동작합니다. PIM은 경로를 생성할 때, 각 라우터에서 멀티캐스트 데이터가 전송되는 인터페이스를 최소화합니다.
* 확장성: PIM은 대규모 네트워크에서도 사용이 가능한 확장성을 가지고 있습니다. 라우팅 프로토콜과 함께 사용됨으로써 대규모 네트워크에서도 라우팅 경로를 생성할 수 있습니다.

PIM 프로토콜은 Sparse mode와 Dense mode 두 가지 모드가 있습니다. Sparse mode는 멀티캐스트 데이터 전송이 적은 경우에 적합하며, Dense mode는 멀티캐스트 데이터 전송이 많은 경우에 적합합니다. 또한, PIM-SM(Protocol Independent Multicast-Sparse Mode)과 PIM-DM(Protocol Independent Multicast-Dense Mode) 두 가지 버전이 있습니다.