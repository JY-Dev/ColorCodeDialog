# ColorCodeDialog
You can get the code value of the color you want. In Android studio

### Library Version

Version v1.0.1

### minSdkVersion

minSdkVersion 21

### Edit Gradle

Edit `YourProject/build.gradle` like below.

#### JitPack
```gradle
allprojects {
    repositories {
        google()
        jcenter()
        maven { url "https://jitpack.io" }
    }
}
```

Edit `app/build.gradle` like below.

```gradle
   implementation 'com.github.JY-Dev:ColorCodeDialog:v1.0.1'
```

## How To Use

### In Code

#### ColorDialog's Constructor
```
ColorDialog(Context,Callback(RedValue : Int,GreenValue :Int, BlueValue:Int, ColorCode:String),InputRedValue:Int,InputGreenValue:Int,InputBlueValue:Int)
Context : Your Activity Context
Callback : It's Dialog Return Callback. Callback provided RGB ColorCode to Int(RedValue,GreenValue,BlueValue) and String(ColorCode) 
Input Init Color : InputRedValue:Int,InputGreenValue:Int,InputBlueValue:Int
```

#### To call the color code dialog
```
private var red = 0;
private var green = 0;
private var blue = 0;

ColorDialog(this,{ red,green,blue,colorCode ->
                this.red = red
                this.green = green
                this.blue = blue
            },red, green, blue)
```



## In application
![](https://github.com/JY-Dev/CertainColorTextView/blob/master/sampleImg.jpg)
