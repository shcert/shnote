# Base64란?

6bit로 데이터를 인코딩 디코딩하기위한 표준이다.

# Base64를 쓰는 이유

Binary 데이터를 모두 영문자로 바꾸기 위해서 사용한다.  
바이너리 형태로 존재할수밖에 없는 데이터들을 강제로 html 문서에 포함시키기 위해서 Base64를 사용한다.  
바이너리 형태의 데이터들을 html, json같은 문자를 다루는 것들에 포함시키기에 여러번 전송을 안해도 되기에 용량은 늘어날지언정 속도는 더 빨라진다.  

`Binary 데이터를 텍스트 기반 규격으로 다룰 수 있기 때문이다`

# Base64 Padding

Base64는 6비트씩 자르는데 만약 6비트를 채우지 못하면 =로 빈칸을 채우는데 이것을 Padding이라 한다.
