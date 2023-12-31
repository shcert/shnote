# BOOTP
부트스트랩 프로토콜(BOOTP)은 워크스테이션을 서버와 연결하기 위한 동적 방법을 제공합니다. 또한 워크스테이션 인터넷 프로토콜(IP) 주소 및 초기 프로그램 로드(IPL) 소스를 할당하기 위한 동적 방법을 제공합니다.

BOOTP는 TCP/IP 프로토콜입니다. 이를 통해 클라이언트는 네트워크의 서버에서 IP 주소와 로드 파일의 이름을 찾을 수 있습니다. 클라이언트는 BOOTP를 사용하여 클라이언트 사용자의 개입 없이 이 정보를 찾습니다.

BOOTP 서버는 DHCP(Dynamic Host Configuration Protocol)도 사용하는 잘 알려진 BOOTP 서버 포트 67에서 수신 대기합니다. 이 때문에 BOOTP와 DHCP는 동일한 시스템에서 동시에 작동할 수 없습니다. (DHCP는 BOOTP 클라이언트를 지원하는 데 선호되는 방법입니다.) 서버가 클라이언트 요청을 수신하면 클라이언트의 IP 주소를 조회하고 해당 클라이언트에 응답을 반환합니다. 이 응답에는 클라이언트의 IP 주소와 로드 파일의 이름이 모두 포함됩니다. 그런 다음 클라이언트는 파일 로드를 위해 서버에 대한 TFTP(Trivial File Transfer Protocol) 요청을 시작합니다.