# react-native-art-wave
[npm](https://github.com/CJELLYS/react-native-art-wave)

[git](https://github.com/CJELLYS/react-native-art-wave)

Use Art to draw waves on both iOS and Android.
## Install 
```
npm install react-native-art-wave
```
<img src="https://github.com/CJELLYS/image/blob/master/androidWave.gif" width="300" />

<img src="https://github.com/CJELLYS/image/blob/master/iosWave.gif" width="300" />

## Usage

```
import React, { Component } from 'react';
import {
  AppRegistry,
  StyleSheet,
  View,
  Dimensions,
} from 'react-native';

import { ArtTest } from "react-native-art-wave"
 
var ScreenWidth = Dimensions.get('window').width;
var ScreenHeight = Dimensions.get('window').height;
export class MyApp extends Component {
  render() {
    return (
      <View style={styles.container}>
       <ArtTest 
       type={"circular"}
       proportion={0.6} 
       surfaceWidth = {300} 
       surfaceHeigth ={300} 
       superViewBackgroundColor={"blue"} 
       style = {{backgroundColor:'#FF7800'}}/>
      </View>
    );
  }
}

const styles = StyleSheet.create({
  container: {
    width: ScreenWidth,
    height: ScreenHeight,
    justifyContent: 'center',
    alignItems: 'center',
    backgroundColor: 'blue',
  },
});
```