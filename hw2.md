<h1>HW2</h1>

   ```swift
import SwiftUI

struct ContentView: View{
    @State var count:Int = 0
    @State var ct:Int = 0
    let countm = ["✂️","🪨","🖐🏽"] 
    let countn = ["🪨", "✂️", "🖐🏽"]
    var body:some View{
        VStack(alignment: .center, spacing: 0){
            Text(countn[count])
                .padding(.all,10)
                .frame(width: 150, height: 80, alignment: .top)
                .font(.system(size: 50))
            Button(action: {
                self.count = Int.random(in: 0...2)},
                   label: {
                Text("開始")
                    .padding(.all,10)
                    .frame(width: 300, height: 80, alignment: .top)
                    .font(.system(size:50))
                    .background(Color.blue)
                    .foregroundColor(.white)
                    .border(Color.blue, width: 5)
                    .cornerRadius(20)
                
            })
            
        }
        
        VStack(alignment: .center, spacing: 0){
            Text(countm[ct])
                .padding(.all,10)
                .frame(width: 150, height: 80, alignment: .bottom)
                .font(.system(size: 50))
            Button(action: {
                self.ct = Int.random(in: 0...2)},
                   label: {
                Text("開始")
                    .padding(.all,10)
                    .frame(width: 300, height: 80, alignment: .center)
                    .font(.system(size:50))
                    .background(Color.red)
                    .foregroundColor(.white)
                    .border(Color.red, width: 5)
                    .cornerRadius(20)
                
            })
            
        }.offset(y:0)
        
    }
    
}
```
<img width="40%"  src="https://github.com/fitdaniel/yzu-swiftui-1101501/blob/main/396579492_650884750495664_5531004924566331748_n.jpg">
