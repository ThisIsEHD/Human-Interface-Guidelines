# Text views

텍스트 뷰는 여러 줄의 스타일링된 텍스트를 표시하며, 이 내용은 선택적으로 편집할 수 있다.

텍스트 뷰는 높이가 동적이며 내용이 뷰 밖으로 빠져나가면 스크롤할 수 있다. 기본적으로 텍스트 뷰 내의 내용은 leading edge에 정렬되며 시스템 레이블 색상을 사용한다. iOS 또는 iPadOS에서 텍스트 뷰를 편집할 수 있을 때 사용자가 텍스트 뷰를 선택하면 키보드가 나타난다.

## Best practices

길이가 길고 편집 가능하거나 특별한 형식으로 텍스트를 표시해야 할 경우 텍스트 뷰를 사용. **텍스트 뷰는 specialized 텍스트를 표시하고 텍스트 입력을 받을 수 있다**는 점에서 ****텍스트 필드 및 레이블과 다르다. 소량의 텍스트를 표시해야 하는 경우 레이블을 대신 사용하거나 텍스트를 편집할 수 있는 경우 텍스트 필드를 사용하는 것이 더 간단하다. 

텍스트의 가독성 (가시성) 을 확보해라. 사용자가 디바이스에서 텍스트 크기를 변경해도 텍스트가 잘 보이도록 다이나믹 타입을 사용하는 것이 좋다. 또한 접근성 옵션이 켜졌을 때 (굵은 글씨 등)의 상황도 테스트해야 하는 것이 좋다. 디테일: [Accessibility](https://developer.apple.com/design/human-interface-guidelines/foundations/accessibility), [Typography](https://developer.apple.com/design/human-interface-guidelines/foundations/typography)
Informative한 텍스트는 선택가능하게 해라. 복붙해서 검색해볼 수 있게.

 

적절한 키보드 타입을 보여라. 데이터 입력을 간소화하려면 텍스트 뷰를 편집할 때 표시되는 키보드가 내용 유형에 적합해야 한 것이 좋다
