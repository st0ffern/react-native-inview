# react-native-inview
Detects if a element is inside a ScrollView or a ListView and reports back.

###Install

```js
npm i -S react-native-inview
```
or with yarnpkg:
```js
yarn add react-native-inview --save
```

###Uage
```
import Inview from 'react-native-inview'

render() {
  return (
  <ScrollView>
    <InViewPort onChange={inView => console.log('Inview: '+ inView)}>
      ....
    </InViewPort>

    <InViewPort onChange={inView => console.log('Inview: '+ inView)}>
      ....
    </InViewPort>

    <InViewPort onChange={inView => console.log('Inview: '+ inView)}>
      ....
    </InViewPort>

    <InViewPort onChange={inView => console.log('Inview: '+ inView)}>
      ....
    </InViewPort>

  </ScrollView>
  );
}
```
