<h1>HW1</h1>

```swift
import SwiftUI

struct ContentView: View{var body:some View{
    Image("Daniel.did")
        .resizable()
        .background(.pink)
        .aspectRatio(contentMode: .fit) .frame(width: 400, height: 350, alignment: .center) 
    
        .overlay(Text("1101501 \n陳楷元Daniel \n 歡迎光臨")
            .fontWeight(.heavy)
            .frame(width: 180, height: 100, alignment: .center)
            .foregroundColor(.white)
            .lineSpacing(8)
            .background(Color.black)
            .opacity(0.7)
            .cornerRadius(30)
                 
                 ,alignment: .bottom
        )
    
    
    
}}
```
<img width="40%"  src="https://github.com/fitdaniel/yzu-swiftui-1101501/blob/main/397979247_315870301259248_8952752190955919943_n.jpg">
