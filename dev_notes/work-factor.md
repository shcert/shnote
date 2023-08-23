# 워크 팩터(Work factor)
는 보안 해시 함수를 사용하여 비밀번호를 저장할 때, 해당 비밀번호를 추측하거나 노출되었을 때에도 비밀번호를 보호하기 위한 보안 강도를 나타내는 값입니다.

보안 해시 함수는 일반적인 해시 함수와는 달리, 입력 데이터를 변형하거나 여러 번 해시하는 등의 복잡한 작업을 수행하여 보안성을 높인 함수입니다. 하지만, 보안 해시 함수로만 비밀번호를 저장하면, 공격자가 무차별 대입 공격 등의 공격을 통해 비밀번호를 노출시키는 경우가 있습니다.

이를 방지하기 위해, 보안 해시 함수를 사용할 때에는 워크 팩터를 설정하여 비밀번호 추측 시간을 늘리는 것이 일반적입니다. 즉, 워크 팩터를 높게 설정할수록 비밀번호를 추측하는 데 필요한 시간이 더 오래 걸리기 때문에, 공격자가 비밀번호를 노출시키는 것을 방지할 수 있습니다.

워크 팩터는 대개 숫자로 표현되며, 숫자가 높을수록 보안 강도가 높아집니다. 하지만, 워크 팩터가 높을수록 해시 함수를 사용할 때 걸리는 시간이 더 많아지기 때문에, 서비스의 성능에도 영향을 미칠 수 있습니다. 따라서, 워크 팩터를 설정할 때에는 보안 강도와 성능 사이에서 적절한 균형을 유지하는 것이 중요합니다.