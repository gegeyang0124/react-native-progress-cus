# react-native-progress-cus
基于[react-native-progress@3.4.0](https://github.com/oblador/react-native-progress)进行修改的，基本遵循其属性和方法设定，主要修改一些方法和渲染逻辑

### 安装
npm i --save react-native-progress-cus

### 修改react-native-progress的内容
1.修改渲染逻辑 <br>
2.修改了Circle的formatText 使其可以传入自定义UI <br>
3.增加属性isCenterDefaultUI:是否使用formatText的默认ui，默认是使用 true；否则false，自定义formatText的UI <br>

### 使用isCenterDefaultUI和formatText (其他属性及使用方法，请查看[react-native-progress@3.4.0](https://github.com/oblador/react-native-progress))
```javascript
import {
    Circle
} from 'react-native-progress-cus';

<Circle size={this.getProgressSize()} // 圆的直径
        style={styles.circleStyle}
        progress={progress||0}
        unfilledColor={unfilledColor} // 剩余进度的颜色
        color={color}
        thickness={this.getThickness()} // 内圆厚度
        showsText={true}
        isCenterDefaultUI={false}
        formatText={this.renderItem}/>)
```

### [我的博客](http://blog.sina.com.cn/s/articlelist_6078695441_0_1.html)
