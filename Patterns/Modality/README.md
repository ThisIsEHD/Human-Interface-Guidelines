# Modality

모달리티는 부모 뷰와의 상호 작용을 방지하고 명시적인 동작을 필요로 하는 별도의 포커스된 모드로 컨텐츠를 제공하는 디자인.

컨텐츠를 모달로 제시했을 때:

- 사용자가 중요한 정보를 받고 필요한 경우 이에 따라 행동하도록 보장
- 사용자가 최근 작업을 확인하거나 수정할 수 있는 옵션 제공
- 사용자가 이전의 맥락을 파악하지 않고 명확하고 좁은 범위의 작업을 수행할 수 있도록 지원
- 복잡한 작업에 집중할 수 있도록 지원

플랫폼(iOS, iPadOS, macOS 등을 말하는 듯) 에 따라 각기 다른 요소를 사용하여 모달을 표시할 수 있다. 예를 들어, iOS, iPadOS 및 macOS 앱은 별도의 작업을 수행하기 위해 sheets 또는 pop over를 주로 사용하지만 macOS 및 iPadOS 앱은 별도의 창을 사용할 수도 있다.

미디어 시청과 같은 일시적인 몰입 경험 또는 콘텐츠 편집과 같은 뚜렷한 멀티스탭 작업에 사람들이 집중할 수 있도록 돕기 위해 전체 화면 모달 경험을 제공할 수 있다.

## Best Practices

- 분명한 이점이 있을 때만 콘텐츠를 모달로 제시. 모달은 맥락을 끊는 경험이기 때문에.
- 모달에서 하는 작업은 단순하고, 짧고, 좁게 집중하는 것을 목표로 한다.
- 모달 작업 내에서 뷰의 계층을 제시하지 마라. 모달은 단순한 작업을 타게팅하므로.
- 몰입형 콘텐츠 또는 복잡한 작업에 전체 화면 모달 스타일을 사용하는 것을 고려해보라.
- 항상 사람들에게 모달 뷰를 없앨 수 있는 분명한 방법을 제공하라.
- 필요한 경우 모달을 닫기 전에 확인을 받아 데이터 손실을 방지할 수 있다. (정말 끝내시겠습니까? 같은거)
- 모달 뷰에 title 등을 달아서 어떤 작업을 하고 있는지 알기 쉽게해라
- 다른 모달  위에 모달 보기를 표시하지 않도록 해라.

합니다. 동시에 화면의 여러 모달 뷰는 사람들이 둘 이상의 이전 컨텍스트를 기억해야 하기 때문에 혼란스러울 수 있다. 중요한 정보를 전달하기 위해 경고가 다른 모든 콘텐츠 위에 나타날 수 있지만 동시에 둘 이상의 경고를 화면에 표시하면 매우 혼란스럽습니다.
