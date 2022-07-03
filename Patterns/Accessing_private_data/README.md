#Accessing private data

## Requesting permission

접근을 위해 허가를 요청해야 하는 것들

- Personal data, including location, health, financial, contact, and other personally identifying information
- User-generated content like emails, messages, calendar data, contacts, gameplay information, Apple Music activity, HomeKit data, and audio, video, and photo content
- Protected resources like Bluetooth peripherals, home automation features, Wi-Fi connections, and local networks
- Device capabilities like camera and microphone
- The device’s advertising identifier, which enables app tracking

시스템은 제작자의 요청을 사용자에게 보여주기 위해 standard alert를 제공한다. 그리고 사용자는 설정의 privacy에서 그 설명을 보거나 그들의 선택에 대한 업데이트를 할 수 있다.

앱이 작동하는데에 필수적인 데이터나 자원이 아니라면 앱을 시작할 때 요구하지 마라

아래와 같이 요구하는 ability, data, resource를 앱에서 어떻게 사용하는지 명확히 밝혀라.

![image](https://user-images.githubusercontent.com/107873842/177046950-2a2fe8a8-6da5-454b-a9be-d2e56e7e5f18.jpeg)

## Location button

iOS 15, iPadOS 15, watchOS 8부터 Core Location은 사용자가 앱이 필요로 하는 순간에 그들의 위치에 접근할 수 있는 임시 권한을 부여할 수 있도록 버튼을 제공한다. 버튼 UI는 앱에 맞게 적절히 아래와 같이 만들 수 있다.

![image](https://user-images.githubusercontent.com/107873842/177046972-a83629fb-235f-4b40-95e2-2092119fd3d0.jpeg)

사용자가 처음 앱을 켜고, 위치 버튼을 탭하면 시스템은 standard alert를 띄운다. 그를 통해 사용자는 앱의 위치 정보에의 접근 제한에 대해 알려주고 위치 정보 공유를 시작했을 때 그들의 위치 정보를 어떻게 보여주는지 알려준다.

![image](https://user-images.githubusercontent.com/107873842/177046999-a030cfaf-4c85-441f-8410-b5efbed77bca.jpeg)

해당 정보를 확인한 후 위치 버튼을 탭하여 1회의 위치 정보로의 접근을 허가한다. 앱 사용을 중지하면 각 일회성 인증이 만료되지만 버튼의 동작에 대한 이해를 재확인할 필요는 없다.

특정 앱 기능 (메시지에 위치정보 첨부하기, 가게 찾기 등) 을 위해 사용자들이 위치버튼을 통해 위치를 쉽게 공유할 수 있는 방법을 고려해봐라

앱의 UI를 고려해서 위치 버튼을 커스터마이징 하는 것을 고려해봐라

- Choose the system-provided title that works best with your feature, such as “Current Location” or “Share My Current Location”
- Choose the filled or outlined location glyph
- Select a background color and a color for the title and glyph
- Adjust the button’s corner radius

위치 버튼에 대한 신뢰도와 인식성을 위해 버튼의 다른 시각적 요소는 커스터마이징 할 수 없다. (적당히 커스터마이징 하라는 얘기인듯) 가독성 없거나, 버튼의 글자가 버튼에 잘 맞지 않는 등의 문제발생이 시스템에 의해 지속적으로 확인된다면 사용자가 위치 버튼을 탭해도 시스템이 그것으로의 접근을 막을 수도 있으니 주의하라.
