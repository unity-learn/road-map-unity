# Road Map Unity

Có phải bạn đang muốn trở thành nhà phát triển Unity. Có quá nhiều kiến thức phải học mà bạn chưa biết bắt đầu từ đâu. Tại đây, tôi sẽ lên một lộ trình giúp bạn nắm được các bước để bắt đầu con đường phát triển trò chơi trên Unity.

## 1. Basic (Cơ bản)

```mermaid
flowchart LR
A[.NET/C#]
B[Unity Basic]
C[Version Control] 
A-->B
A-->C-->D[Git/GitHub]
E["Scenes<br>GameObjects<br>Prefabs<br>MonoBehaviour<br>Components"]
B-->E 

```
### .Net
- Bởi vì Unity sử dụng nền tảng .Net, nên bạn hãy tìm hiểu sơ lược về .Net để biết được Unity đã tích hợp .Net như thế nào? Nhằm mục đích gì? Có ưu điểm và hạn chế nào?
### C#
- Vì sao lại là C# mà không phải là ngôn ngữ khác? Có lẽ điều này cũng chẳng quan trọng lắm vì mình chỉ cần biết là Unity chọn C# thì chúng ta sẽ học C# =)))
- Đối với một số anh em đã làm quen hoặc biết các ngôn ngữ lập trình như C, C++ thì việc làm quen với C# sẽ nhẹ nhàng hơn rất nhiều. Còn những anh em chưa có bất kì kiến thức nào thì hãy bắt đầu từ `C# Tutorial` (`Input/Output`, `Variables`, `Data Types`, `While/For Loop`, `If/Else`, `List/Arrays`, `Math`, ...), Sau khi hiểu cơ bản phần `Tutorial` thì bạn sẽ chuyển qua `C# - OOP` (`Classes/Objects`, `Constructors`, `Access Modifiers`, `Properties and Encapsulation`, `Inheritance`, `Polymorphism`, `Abstraction/Interface`, ...). Mình nghĩ sau khi nắm vững chừng đó kiến thức về C# là bạn đã có thể tự tin bắt đầu với Unity rồi.
- Hãy bắt đầu với [C# cơ bản](https://github.com/unity-learn/basic-csharp-for-unity)
### Unity Basic
- Lần đầu mở Unity Editor lên bạn sẽ thấy rất nhiều cửa sổ được bung ra, và bạn không biết nhiệm vụ của từng cửa sổ đó là gì. Vì thế, bạn sẽ cần tìm hiểu sơ qua về giao diện của Unity Editor và biết được nhiệm vụ của các cửa sổ cơ bản (`Project`, `Console`, `Hierarchy`, `Scene`, `Game`, `Inspector`).
- Tiếp theo bạn sẽ tìm hiểu về `Scenes`, `GameObject`, `Prefabs`, `MonoBehaviour`, và các `Components` phổ biến như `Transform`, `RigidBody`, `Collider`, ...
- Sau đó bạn sẽ đến giai đoạn sử dụng script được viết bằng C# để viết ra những thứ logic nhiệm màu cho sản phẩm game của mình. Đây là giai đoạn cần sự tích cực tìm tòi nghiên cứu để bạn có thể tích trữ cho bản thân một khối lượng kiến thức, kỹ năng xử lý vấn đề và bạn sẽ làm ra những sản phẩm game tốt hơn theo thời gian.
### Version Control
- Bạn sẽ cần một kho lưu trữ dự án (bao gồm asset game như sprite, model, sound, ... và mã nguồn), bạn cần công cụ hỗ trợ để tất cả mọi người trong nhóm có thể làm việc trên cùng một dự án mà không bị xung đột, bạn cần một công cụ ghi nhớ tất cả sự thay đổi trong dự án của mình, ...
- Ở đây mình chọn [Git/GitHub](https://github.com/unity-learn/Getting-Started-with-Git) là công cụ quản lý và lưu trữ mã nguồn, nó sẽ giúp bạn xử lý tất cả các vấn đề nêu trên và còn nhiều hơn thế nữa. Bạn có thể tìm hiểu cách sử dụng Git/GitHub hoặc bất cứ công cụ nào tương tự phù hợp với bạn.

## 2. Visual (Thị giác)
```mermaid
flowchart TD
Visual
A["Unity UI <br> UI Elements <br> TextMeshPro <br> ..."] --UI-->Visual
B["Lighting<br>Shaders<br>Shader Graph<br> ..."] --"2D/3D"--> Visual
C["Animation<br>Animator<br>Timeline<br>Tween<br>..."] --Animation-->Visual
```

### UI
- Unity UI, TextMeshPro,... không khó để tìm hiểu và làm quen với nó, xem [tại đây](https://learn.unity.com/mission/61a63fbcedbc2a0020607294?pathwayId=61a65568edbc2a00206076dd)
### 2D/3D
- Bạn cần hiểu về Lighting và cách nó hoạt động,  bạn có thể xem [tại đây](https://learn.unity.com/mission/creative-core-lighting?pathwayId=61a65568edbc2a00206076dd)
- Shader và ngôn ngữ shader. Bạn có thể tìm hiểu về phần này, nhưng mình thấy nó khá khó nhằn nên mình thường tìm kiếm các shader có sẵn hoặc sử dụng chat GPT để tạo shader mong muốn.
- Shader Graph để lập trình shader trực quan mà không phải code, xem [tại đây](https://learn.unity.com/tutorial/introduction-to-shader-graph#)
### Animation
- Animation và Animator là những thành phần cơ bản của Unity, xem [tại đây](https://learn.unity.com/mission/61a64e25edbc2a0020607564?pathwayId=61a65568edbc2a00206076dd)
- Timeline phù hợp với các tình huống tạo một cảnh dài bao gồm nhiều hoạt ảnh, âm thanh, ...
- Tween: Tìm hiểu [DOTween](https://dotween.demigiant.com/), [PrimeTween](https://github.com/KyryloKuzyk/PrimeTween), [LitMotion](https://github.com/AnnulusGames/LitMotion), ... Tất cả đều rất tuyệt vời. Hãy chọn một loại phù hợp với bạn nhất

## 3. Project Architecture (Kiến trúc)

```mermaid
flowchart TD
p[Project Architecture]
b["SOLID<br>KISS<br>DRY<br>..."] --Design principles-->p
c["Singleton<br>Observer"<br>State<br>Strategy<br>Command<br>ObjectPool<br>...]--Design patterns-->p
a["<a href='https://uniandes-se4ma.gitlab.io/books/chapter8/mvc-mvvm-mv-mvwhat.html'>MC* Patterns"</a><br>Dependency injection<br>OOP<br>ECS<br>...]--Architectural Patterns-->p
```

### Architectural patterns
- Tìm hiểu về một số nguyên tắc lập trình như: Lập trình hướng đối tượng (OOP), Thiết kế hướng dữ liệu (DOD), ...
- Tìm hiểu các mẫu [MV*](https://uniandes-se4ma.gitlab.io/books/chapter8/mvc-mvvm-mv-mvwhat.html) (MVC, MVP, MVVM) rất hữu ích
- Để triển khai dependency injection, hãy tìm hiểu về [DI và IoC](https://www.amazon.com/Dependency-Injection-Principles-Practices-Patterns-dp-161729473X/dp/161729473X) . Một khuôn khổ DI được sử dụng rộng rãi cho Unity là [Zenject](https://github.com/modesttree/Zenject)
- Đối với phát triển trò chơi cốt lõi, phương pháp Entity Component System (ECS) hiện đang phổ biến nhất. Bạn có thể sử dụng [Unity DOTS](https://unity.com/dots) hoặc các triển khai khác mà bạn thích.
### Các mẫu thiết kế
- Singleton
- Observer
- State
- Command
- ObjectPool
- Strategy
### Các nguyên tắc thiết kế
- SOLID
- KISS
- DRY

## 4. Next level (cấp độ tiếp theo)
Đây là cấp độ không cần thiết đối với bạn nếu như bạn là người mới bắt đầu. Tuy nhiên, bạn vẫn sẽ phải tìm hiểu về nó sớm hay muộn.
- Khi bạn thấy game của mình khá lớn và nó bắt đầu xuất hiện tình trạng bị trễ, thậm chí bị văng ra ngoài, thiết bị của bạn thì nóng lên, .... Lúc này, bạn cần tìm hiểu các phương pháp để tối ưu hiệu năng cho game của bạn (optimizations). Hãy kiểm tra [Profiler](https://docs.unity3d.com/Manual/Profiler.html) và [Memory profiler](https://unity.com/how-to/use-memory-profiling-unity) nó sẽ giúp bạn rất nhiều trong việc tìm ra nguyên nhân gây ra các vấn đề trên.
- Tìm hiểu và tích hợp các công cụ quảng cáo như [AdMob](https://github.com/googleads/googleads-mobile-unity), [Max](https://github.com/AppLovin/AppLovin-MAX-Unity-Plugin), ... hoặc các công cụ Tracking như [Firebase](https://github.com/firebase/firebase-unity-sdk), [Adjust](https://github.com/adjust/unity_sdk) hay [AppsFlyer](https://github.com/AppsFlyerSDK/appsflyer-unity-plugin?tab=readme-ov-file)
