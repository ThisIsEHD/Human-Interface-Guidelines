# Navigation bars

네비게이션 바는 앱 화면 상단에 탐색 막대이며 콘텐츠 계층을 통해 탐색을 가능케 한다.

또한 여기서 제목을 자연스럽게 표시할 수 있다. 앱이나 게임에서 사용자가 현위치를 알 수 있게 하며 화면 내용에 영향을 주는 컨트롤이(navi bar item 등?) 포함될 수 있다.

## Best practices

화면 제목을 간결하게 작성해라. 15자 이하로 해서 컨트롤을 위한 충분한 공간을 남기는 게 좋음.

보다 몰입감 있는 경험을 위해 네비게이션 바를 일시적으로 숨길 수도 있다. 예를 들어, 사진볼 때.

표준 뒤로가기 버튼을 사용해라. 커스텀해서 만들거면 뒤로가기 버튼임이 명백하게, 사용자가 예상하는대로 동작하게끔, 앱의 여타 인터페이스와 통일성 있으며, 앱 전체에서 일관적으로 동작하는 지 확인해야.

네비게이션 바에서 아래와 같이 segmented control을 사용하여 동등한 계층으로 만드는 것을 고려해라. 예를 들어, 전화기 앱에서 segmented control을 사용하여 사람들이 최근 통화 보기 또는 부재중 통화만 볼 수 있도록 합니다. 앱에서 이와 같은 설계가 타당하다면 최상위의 네비게이션 바에만 segmented control을 배치하고 2단계 화면부터는 백 버튼을 생성해야 한다. 디테일: [Segmented controls](https://developer.apple.com/design/human-interface-guidelines/components/selection-and-input/segmented-controls)

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/9598c8e5-5500-442d-8ec4-aab3d2771506/Untitled.jpeg)

네비게이션 바의 Large title은 사용자가 내용을 스크롤하기 시작하면 standard title로 전환되고, 맨 위로 스크롤하면 다시 커진다.

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/d1ac1279-c7ad-45f6-b710-7a38c2d83d12/Untitled.jpeg)

타이틀과 컨텐츠 간의 연결성을 자연스럽게 하고 싶다면 large title navigation bar의 테두리를 숨기는 것이 좋다. 그러나 테두리가 없으면 네비게이션 바의 타이틀과 버튼을 구분하기 어려울 수도 있으니 주의해야 한다. 반면 iPad의 스플릿 뷰에서는 borderless 스타일을 사용하여 primary view, secondary view 간의 일관성을 유지할 수 있다. 막대의 그림자를 제거하여 네비게이션 바 아래쪽 테두리를 숨길 수 있고 사용자가 컨텐츠 영역을 스크롤하면 테두리가 자동으로 다시 나타난다.
