# Tab bars

탭 바는 bar items를 사용하여 동일한 뷰에서 서로 배타적인 내용 창 사이를 이동한다.

탭 바는 뷰가 제공하는 다양한 유형의 정보 또는 기능을 이해하는 데 도움이 된다. **또한 각 섹션 내의 현재 탐색 상태를 유지하면서 사용자가 뷰 섹션을 빠르게 전환할 수 있다.**

## Best practices

- 탭 바를 사용할 때는 탐색의 용이성을 위해 사용하는 것이지 특정한 액션을 호출하기 위해 하는 것이 아니다. 현재뷰에 특정 액션을 부여해야하는 경우 탭바가 아니라 Tool bar를 사용해라.
- 앱에서 다른 영역으로 이동할 때 탭 바가 보이도록 하라. 모달 뷰 내의 탭 바는 예외.
- 웬만하면 탭의 수를 3~5개로 적게 유지해라. ipadOS, tvOS에서는 좀 더 많아도 괜찮다. 많으면 복잡해질 뿐이다.
- 특정 탭 내의 컨텐츠가 unavailable 해도 탭을 보여주고 인터랙션이 가능하게 유지하고 해당 탭 내에서 할 것이 만약 없다면 다른 대안을 제시하라. 예를 들어, music 앱에 노래가 없다면 해당 탭 내에서 새로운 음악을 다운받으라고 제안하라.
- 최대한 구체적이지만 짧은 명사나 동사를 탭 제목으로 사용하라.
- 특정 탭이 과밀하지 않도록 주의하라. 예를 들어 "홈" 탭은 범위가 너무 크다. 구체적 기능을 하나의 탭에 담는 것을 목표로 하라.

- 기본적으로 탭 바는 반투명한다. It uses a background material only when content appears behind it, removing the material when the view scrolls to the bottom. 키보드가 화면에 있으면 탭 바는 숨는다.
- 웬만하면 오버플로우 탭 (제일 오른쪽에 땡땡땡 있는 More tab)을 사용하지 마라
- iPadOS 앱에서 탭 바 대신 사이드바를 사용하는 것을 고려하라 그게 더 많은 탭을 표시 할 수 있다.
- **Ensure that tabs affect the view that’s attached to the tab bar, not views elsewhere onscreen.** For example, make sure selecting a tab on the left side of a split view doesn’t cause the right side of the split view to change. (iPadOS 얘기인듯?)
- 나대지 않으면서(?ㅋㅋㅋㅋ) 사용자에게 정보를 주려면 뱃지를 사용해라. 예를 들어, 탭바에 빨간색 뱃지 등을 사용하여 새로운 정보의 업데이트 등을 얌전히(ㅋㅋㅋ) 알릴 수 있다.
- SF symbol을 사용하여 확장 가능하고 시각적으로 일관된 탭 바 아이템을 제공하는 것을 고려하라. SF symbol을 사용하면 탭 바 아이템이 자동으로 다른 컨텍스트에 맞게 조정됩니다.(장치별, 가로세로 모드 별 등). 또한 세로 모드일 때는 symbol이 제목 위에 나타날 수 있지만 가로 방향에서는 symbol과 제목이 나란히 나타날 수도 있다.

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/069f8952-19bd-4dac-b8b8-adf3f780e4c2/Untitled.jpeg)

규격에 대해서는 원문 참조: [https://developer.apple.com/design/human-interface-guidelines/components/navigation-and-search/tab-bars](https://developer.apple.com/design/human-interface-guidelines/components/navigation-and-search/tab-bars)
