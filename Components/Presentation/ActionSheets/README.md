# Action sheets

액션 시트는 사용자가 시작한 작업과 관련된 선택 사항을 표시.

When you use SwiftUI, you can enable action sheet functionality in all platforms by specifying a [presentation modifier](https://developer.apple.com/documentation/swiftui/view-presentation) for a confirmation dialog. If you use UIKit, you use the [actionSheet](https://developer.apple.com/documentation/uikit/uialertcontroller/style/actionsheet)
 style of [UIAlertController](https://developer.apple.com/documentation/uikit/uialertcontroller) to display an action sheet in iOS, iPadOS, and tvOS.

## Best practices

알림이 아닌 액션 시트를 사용하여 의도적인 수행과 관련된 선택사항을 제공하라. 알림은 또한 파괴적인 결과를 초래하는 작업을 확인하거나 취소하는 데 좋지만 작업과 관련된 추가 선택사항 제공에는 적절치 않다. 

액션 시트는 꼭 필요할 때 가끔 사용하라. 현재의 작업을 방해하기 때문.

각 제목을 한 줄에 표시할 수 있을 정도로 짧게 유지.

필요한 경우 데이터 삭제가 가능한 작업을 거부할 수 있는 “취소” 단추를 제공하라. Cancel(취소) 버튼을 액션 시트의 하단(또는 watch OS에서 시트의 왼쪽 상단 모서리)에 놓아라. 

destructive한 선택을 시각적으로 두드러지게 하라.

iOS, iPadOS

메뉴가 아닌 액션 시트를 사용하여 액션 관련된 선택사항을 제공하라. 사용자는 명확한 선택이 필요할 수 있는 작업을 수행할 때 액션 시트가 나타나는 것에 익숙하다. *대조적으로, 사람들은 그것을 공개하기로 선택했을 때 메뉴가 나타나기를 기대한다.(메뉴…?)*

수행 시트가 스크롤되지 않도록 해라.
