<h1>HW3</h1>

   ```swift
import SwiftUI


struct ContentView: View {
    var body: some View {
        VStack{
            TitleView()
            HStack{
                bearView(imageName: "Lebron")
                bearView(imageName: "Wade")
                bearView(imageName: "Kd")
                 
                 
            }
            HStack{
                bearView(imageName: "Kobe")
                bearView(imageName: "O’Neal")
                bearView(imageName: "Pg")
            }
            HStack{
                bearView(imageName: "Duncan")
                bearView(imageName: "Wall")
                bearView(imageName: "Rose")
            }
            
        }
    }
}
struct ContentView_Preview: PreviewProvider {
    static var previews: some View {
        ContentView()
    }
}

struct TitleView: View {
    var body: some View {
        VStack(alignment: .center, spacing: 2){
            Text("Daniel的收藏櫃")
                .font(.system(size: 30))
                .foregroundColor(Color(red: 200/255, green: 190/255, blue: 29/255))
        }
    }
}


struct lbj: View {
    var body: some View {
        VStack{
            Image("Lbj")
                .resizable()
                .aspectRatio(contentMode:.fit)
                .padding(.all, 2)
            Text("lebron")
                .fontWeight(.bold) 
            .font(.system(size: 15))}
    }
}

struct wade: View {
    var body: some View {
        VStack{
            Image("Wade")
                .resizable()
                .aspectRatio(contentMode:.fit)
                .padding(.all, 2)
            Text("wade")
                .fontWeight(.bold)
            .font(.system(size: 15))}
    }
}
struct kd: View {
    var body: some View {
        VStack{
            Image("Kd")
                .resizable()
                .aspectRatio(contentMode:.fit)
                .padding(.all, 2)
            Text("KD")
                .fontWeight(.bold)
            .font(.system(size: 15))}
    }}
struct kobe: View {
    var body: some View {
        VStack{
            Image("Kobe")
                .resizable()
                .aspectRatio(contentMode:.fit)
                .padding(.all, 2)
            Text("Kobe")
                .fontWeight(.bold)
            .font(.system(size: 15))}
    }}
    

extension UIScreen{
    static let screenwidth = UIScreen.main.bounds.size.width
    static let screenheight = UIScreen.main.bounds.size.height
    static let screensize = UIScreen.main.bounds.size
    
}


struct bearView: View{
    var imageName:String
    var body: some View{
        VStack{
            Image(imageName)
                .resizable()
                .aspectRatio(contentMode:.fit)
                .frame(height: 180,alignment: .center)
            Text(imageName.capitalized)
                .fontWeight(.bold)
            .font(.system(size: 15))}
        .frame(minWidth: 0, idealWidth: 100, maxWidth: .infinity, minHeight: 0, idealHeight: 100, maxHeight: .infinity, alignment: .center)
    }}

 ```
<img width="40%"  src="https://github.com/fitdaniel/yzu-swiftui-1101501/blob/main/370089900_276748648681115_7208990384239590077_n.jpg">
