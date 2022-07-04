# Accessibility

Disability를 가진 사람을 포함하여 모든 사람들에게 접근성있는 디자인을 해야한다. 그를 위해 지켜야 하는 원칙들

- 단순하게
- 다양한 감각을 이용하여 감지할 수 있게
- 개인화를 제공하며
- 접근성을 위해 검사하고 테스트해야 한다

Xcode’s Accessibility Inspector를 는 검사와 테스트를 도와줌

## Interactions

Assistive tech는 사용자와 기기 간의 상호작용을 확장시킨다.

## Gestures

Platform gestures를 덮어쓰지 말 것. 사람들이 기대하는 기능이 있기 때문.

공통된 상호작용에 대해 단순한 제스쳐를 사용할 것.

동작기반 actions에 대해서는 대안을 제공할 것. 그것이 불편한 사람이 있을 수 있음.

가능하면 앱의 핵심기능을 여러 물리적 방법을 통해 접근 가능케 할 것.

Drag and Drop 기능을 앱 내에서 가능케 할 것.

## Buttons and Controls

44x44pt 크기 이상으로 컨트롤 및 interactive element를 만들 것

커스텀 요소들의 접근성을 명시하라. (버튼으로 작동하는 view를 위해 button이나 NSAccessibilityButton 등의 system API를 사용 하는 등)

버튼 간의 상대적 중요성을 암시하기 위해 일관된 계층 스타일을 사용해라

웬만하면 시스템이 제공하는 switch 를 사용해라

링크를 제공할 때는 컬러와 더불어 밑줄과 같은 가시적 지표를 제공해라

## User input

사용자가 글로 쓰기 보다는 말하여 정보를 입력하도록 해라. (텍스트 입력 필드에 dictation 버튼 등을 추가하여)

시리 또는 단축키를 제공하여 목소리 만으로 중요기능을 할 수 있도록 해라

웬만하면 사용자가 평문을 선택하는 것을 막지 마라

## Haptics

시스템 상 정의된 햅틱을 지원하라. 볼 수 없는 상황에서 많은 사람들이 그것에 의지한다.

## VoiceOver

보이스오버는 볼 수 없는 사람들이 정보에 접근하고 그것을 얻는 것을 돕는다

## Content descriptions

의미를 전달하는 이미지들에 대해서는 그것을 대체하는 알맞은 설명을 제공하라. (못 보는 사람들이 VoiceOver 사용할 수 있게)

그것이 전달하는 의미에 맞게 간결한 설명을 제공해서 시각화된 데이터에 대해 접근 가능케 해라.

별 의미 없는 이미지라면 assistive tech에서 제외시켜라

각 스크린에 고유의 타이틀과 제목을 부여하여 정보의 계층을 확보해라

적절한 설명 등을 통해 모든 사람들이 비디오와 오디오를 알아 들을 수 있도록 해라

## Navigation

VoiceOver 사용자들이 모든 요소에 접근할 수 있도록 해라. 커스텀할 경우 [Accessibility modifiers](https://developer.apple.com/documentation/swiftui/view-accessibility) 를 통해 그들이 접근할 수 있도록 도와라.

화면 상의 요소들이 어떻게 묶여있고 정렬되어 있고 링크되어 있는지 명확히 하여 VoiceOver 사용자 경험을 극대화할 수 있게 해라.

화면상의 컨텐츠나 레이아웃이 변경될 때 VoiceOver로 알려주어라.

새로운 웹페이지나 앱을 여는 작업을 하는 control에 대해 사람들이 그것을 예측할 수 있게 해라. (버튼의 타이틀이나 디자인을 달리 한다던지)

중요한 인터페이스 요소들에 대해 그것을 대체할 수 있는 텍스트 레이블을 제공해라. 그것이 화면상 보이지는 않지만 VoiceOver가 읽을 수 있음

필요하다면 VoiceOver Rotor (양 손가락을 화면에 놓고 돌리면 한칸씩 돌아가는 회전자 같은 걸 iOS에서 제공. 오… 애플… 진심이구만) 를 제공하라. ([UIAccessibilityCustomRotor](https://developer.apple.com/documentation/uikit/uiaccessibilitycustomrotor), [NSAccessibilityCustomRotor](https://developer.apple.com/documentation/appkit/nsaccessibilitycustomrotor) 참고)

ipadOs와 macOS에서는 사람들이 키보드로 모든 온스크린 요소에 접근 가능케 해라

## Text display

iOS, iPadOS, tvOS, watchOS에서 Dynamic Type을 지원하고 나의 앱이 모든 폰트를 잘 지원하는지 확인해라

폰트사이즈가 커질 때 텍스트 잘림을 최소화 하라

큰 폰트 사이즈에 대해서는 adjusting layout을 고려하라

폰트사이즈가 커질 때 의미 있는 인터페이스 아이콘들 역시 사이즈를 키워라

폰트사이즈와 관계 없이 한결같은 정보 계층을 유지하라

Regular 또는 heavy 폰트를 사용해서 가시성을 높여라

사용자가 bold text를 사용할 때 그것에 잘 대응할 수 있도록 확인하라

커스텀 폰트를 명확히 읽을 수 있도록 해라

텍스트의 양쪽 정렬을 피해라. 읽기 어렵다.

긴 글에는 이탈릭체나 전부 대문자를 쓰는 것을 피해라

## Color and effects

색깔만으로 오브젝트나 중요한 정보들을 구별하지 마라. Label이나 서체 등을 통해 명확히 알 수 있도록 해라

텍스트에 시스템 컬러를 사용해라

색 조합만으로 두가지 상태나 값을 구분하지 마라. 색맹들은 잘 구분 못함

다크모드에 대응할 수 있도록 뷰를 짜라

대비가 강한 색을 통해 가독성을 높여라

반드시 필요치 않다면 애니메이션을 넣지 말라

‘움직임 최소화’가 켜져 있을 때를 위해 한결 간결한 애니메이션을 제공하라. 

- Tighten springs to reduce bounce effects or track 1:1 with the user’s finger
- Avoid animating depth changes in z-axis layers
- Avoid animating into or out of blurs
- Replace a slide with a fade to avoid motion

사용자가 비디오나 모션 효과를 제어할 수 있도록 해라

움직이거나 깜빡이는 요소를 보여줄 때는 그것이 사용자의 집중을 분산할 수 있기에 주의하라

‘투명도 최소화’에 따라 투명도, blur도(?)를 바꿔라
