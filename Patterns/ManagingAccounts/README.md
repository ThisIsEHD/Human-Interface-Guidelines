# Managing accounts

사용자 경험에 불필요한 장애물만 되지 않는다면 계정은 사용자들이 그들의 컨텐츠와 개인정보를 추적하는 데 편리함을 제공할 수 있다.

핵심기능 관련, 반드시 필요할 때에만 계정을 생성하도록 하고 그렇지 않은 경우는 로그인 없이 앱을 사용할 수 있게 해라.

## Best practices

계정 생성의 장점과 가입 방법을 설명해라. 로그인 화면 등에 메시지를 띄우면 됨.

로그인 없이도 많은 기능을 사용할 수 있게 해라. 너무 처음부터 회원가입, 로그인을 요구하면 사용자는 앱을 지워버리는 경우가 많다. 

‘애플 계정으로 로그인 하기’를 사용하지 않는다면 웬만하면 passkey를 사용해라. passkey는 계정 생성 및 인증을 간소화하여 사용자가 암호를 만들거나 입력할 필요가 없다. 앱이 passkey를 활성화하면 사람들은 새 계정을 만들거나 기존 계정에 로그인할 때 사용자 이름을 제공하기만 하면 된다.([Supporting passkeys](https://developer.apple.com/documentation/authenticationservices/public-private_key_authentication/supporting_passkeys)) 암호를 계속 사용해야 하는 경우 [Password AutoFill](https://developer.apple.com/documentation/security/password_autofill/)을 사용하여 암호 및 보안 코드 정보를 자동으로 생성하고 입력하라.

제공하는 인증방법에 대해 사용자에게 명확히 알려줘라 (’로그인’ 대신 ‘FaceID로 로그인’ 이런 식으로)

디바이스의 사용환경에 맞는, 가능한 인증방법을 사용해라. (페이스, 터치 아이디 구분 / [LABiometryType](https://developer.apple.com/documentation/localauthentication/labiometrytype) 참고)

일반적으로 생체인증 선택이라는 앱 내 설정을 제공하지 않도록 해라. (많이들 하는 것 같던데…)

사용자가 앱 내에서 재사용하는 걸로 착각할 수 있으니, 계정 인증을 위해 passcode라는 이름을 사용하지 마라

## Deleting accounts

> 🚨법적 요구 사항으로 인해 앱이 디지털 건강 기록과 같은 계정이나 정보를 유지 관리하거나 특정 계정 삭제 프로세스를 따라야 하는 경우, 사용자가 유지해야 하는 정보나 계정 및 따라야 하는 프로세스를 사람들이 이해할 수 있도록 상황을 명확하게 설명하라.
> 

계정 삭제 방법을 명확하게 제공해라. 앱내에서 해당 기능을 제공하지 않는다면 잘 보이는 곳에 탈퇴 링크를 첨부해라.

사용자가 ‘애플 아이디로 회원가입’을 이용해서 앱에 가입했다면 계정 삭제시 관련된 토큰을 삭제해라. ([Revoke tokens](https://developer.apple.com/documentation/sign_in_with_apple/revoke_tokens) 참고)

앱, 웹 등에서 동일한 삭제 경험을 유지해라. 둘 중 뭘 더 길게 하지 말라는 얘기인 듯.

계정삭제 예약 기능을 고려해 봐라. 그리고 해당 기능을 제공한다면 당장 삭제할 수 있는 방법도 제공해라.

계정삭제완료시점에 대해 안내하고 그것이 실제로 완료 했을 때 공지해라

인앱 결제를 제공한다면 계정삭제시 아래와 같이 지불과 환불이 어떤식으로 이뤄지는 지 안내해라.

- 자동 갱신형 구독에 대한 청구는 계정 삭제 여부와 상관없이 사람들이 구독을 취소할 때까지 애플을 통해 계속된다.
- 계정을 삭제한 후, 사람들은 구독을 취소하거나 환불을 요청해야 한다.

구독 취소방법과 구매내역 관리 방법에 대해 정보를 제공해라 (For guidance, see [Helping people manage their subscriptions](https://developer.apple.com/design/human-interface-guidelines/technologies/in-app-purchase/auto-renewable-subscriptions/#helping-people-manage-their-subscriptions) and [Providing help with In-App Purchases](https://developer.apple.com/design/human-interface-guidelines/technologies/in-app-purchase/introduction/#providing-help-with-in-app-purchases))
