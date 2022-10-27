# Image views

이미지뷰는 투명하거나 불투명 배경에 단일 이미지(경우에 따라서는  움직이는 것 같은 일련의 이미지들을 -animated sequence of images-)를 표시한다.

이미지뷰 내에서 이미지를 특정 위치에 맞게 확장, 축소, 크기 조정 또는 고정할 수 있다. 이미지 뷰는 일반적으로 상호 작용하지 않는다.

## Best practices

뷰의 주요 목적이 단순히 이미지를 표시하는 것일 때 이미지 뷰를 사용한다. 이미지를 interactive하게 만들려는 경우에는 시스템이 제공하는 버튼에 이미지를 넣는 것이 이미지뷰를 버튼화 하는 것 보다 낫다.

인터페이스에 아이콘을 표시하려면 이미지 뷰 대신 symbol 또는 인터페이스 아이콘(SF symbols 말하는 듯 - 맞네 -)을 사용해라. SF 심볼은 다양한 색상과 불투명도로 렌더링할 수 있는 유선형의 벡터 기반 이미지의 큰 라이브러리를 제공한다. 인터페이스 아이콘(글립 또는 템플릿 이미지라고도 함)은 일반적으로 투명하지 않은 픽셀에 색을 입힐 수 있는 비트맵 이미지이다. symbols와 인터페이스 아이콘은 모두 색상을 조절할 수 있다.

## Content

이미지 뷰에는 PNG, JPEG 및 PDF와 같은 다양한 형식의 풍부한 이미지 데이터가 포함될 수 있다.
이미지에 텍스트를 오버레이할 때 주의. 이미지 위에 텍스트를 합성하면 이미지의 선명도와 텍스트 가독성이 모두 저하될 수 있으므로 텍스트와 이미지가 잘 대비되도록 하고 텍스트 그림자나 배경 레이어를 추가하는 등 텍스트의 가독성을 확보해라.
**Aim to use a consistent size for all images in an animated sequence.** When you prescale images to fit the view, the system doesn't have to perform any scaling. In cases where the system must do the scaling, performance is generally better when all images are the same size and shape.
