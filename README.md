# IceBoxOrganizer

- 패스트 캠퍼스에서 진행한 팀 해커톤 프로젝트 2차
- 냉동 냉장별로 음식물을 저장하여 유통기한을 파악할 수 있고 구매한 물품을 편리하게 정리할 수 있도록 관리하고 싶어서 개발

## Description

- 개발 기간: 2020.02.06 - 2020.02.07 (2일)

- 참여 인원: iOS 2명

- 담당 구현 파트

  - 구현에 필요한 Asset 수집 (런처스크린 이미지, 냉동냉장화면, 음식 아이콘 등)

  - Detail 화면 UI

    

## 시연 영상

|                             시작                             |                             수정                             |                             삭제                             |                             추가                             |
| :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
| ![](https://user-images.githubusercontent.com/57210827/85848495-33573080-b7e4-11ea-8113-eab2d44ba213.gif) | ![](https://user-images.githubusercontent.com/57210827/85848535-4538d380-b7e4-11ea-83bc-03894c48e2ed.gif) | ![](https://user-images.githubusercontent.com/57210827/85848595-626da200-b7e4-11ea-9acb-03a2710f0c02.gif) | ![](https://user-images.githubusercontent.com/57210827/85848625-71545480-b7e4-11ea-81ec-8e5f919081e2.gif) |



* 시작 : 앱델리게이트에서 런치스크린을 사용하지 않고 구현

```swift
DispatchQueue.main.asyncAfter(deadline: .now() + 1) {
      self.window?.rootViewController = rootViewController
      UIView.animate(withDuration: 0.8) {
        self.window?.rootViewController?.view.alpha = 1
      }
    }
```

