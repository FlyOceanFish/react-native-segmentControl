# react-native-segmentControl
like ios UISegmentControl

## 效果图
![EF58B8ED-99B1-43CC-B69D-9135B5A8E39D.png](http://upload-images.jianshu.io/upload_images/6644906-8317d708c7570d91.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
## 使用方法
```javascript
<FOFSegmentControl
    titles={['正在热映','Top250','即将上映']}
    onPress={(i)=>{
    //do something
    }}
/>
````
### 实时刷新index(change the current index any time)
````
<FOFSegmentControl
    selectedIndex={this.state.index}
/>
````
## Props
 Name | Description | Default | Type
:-:|:-:|:-:|:-:
titles | 标题数组  | `['正在热映','Top250','即将上映']` | array
titleStyle|默认标题的Style|`{fontSize:17,textAlign:'center'}`,|style
selectedTitleStyle|选中时标题样式||style
onPress|每个segment点击是的回调||func
selectedIndex|默认选中值|0|number
renderTitle|自定义segment视图||func
underlayColor|点击时高亮颜色|transparent|string
barPosition|scrollBar的位置,分为bottom和top|bottom|string
barColor|scrollBar的颜色|red|string
barWidth|scrollbar的宽度|70|number
