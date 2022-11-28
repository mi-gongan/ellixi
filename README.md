# Ellixi

dreamplus hackerthon에서 account abstraction을 이용한 게임 sdk demo입니다.

## account abstraction

https://eips.ethereum.org/EIPS/eip-4337
: 비탈릭 부레린이 제안한 효과적인 CA 구현 방식

## sdk 설명

: web3 game을 좀 더 native하게 ux를 개선할 수 있는 방법들을 고안
: account abstraction으로 in app wallet을 만든다.

1. session

- 일정 기한동안 싸인을 하지 않도록 설정할 수 있게 함
- 보안적 이슈가 있다고 생각할 수 있지만 단지 in app에서 게임을 할때만 사용하기 때문에 금전적 문제 x

2. paymater

- 가스비를 대신 내줄 수 있음
- ether말고도 erc20으로도 가스비를 낼 수 있다.

3. guardian

- 2차 계정 또는 가족들 계정을 사용하여 내 계정을 복구할 수 있다.

## demo

: https://ellixi.vercel.app/

## 사용한 것

- wagmi (ethereum react hook)
- cupcake(provider wrapper)
  : tx를 user operation으로 추상화 해줍니다. bundler와 소통하기 위함.
- webauthn (지문로그인)
- 그외 (tailwind, framer 등등)
