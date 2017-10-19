# react-native-inview

[![Greenkeeper badge](https://badges.greenkeeper.io/stoffern/react-native-inview.svg)](https://greenkeeper.io/)
Detects if a ScrollView or ListView element is inside the users viewport and reports back on changes

##Install

```js
npm i -S react-native-inview
```
or with yarnpkg:
```js
yarn add react-native-inview --save
```

##Props
- `onChange` **(required)**: callback function that report true or false if component is in view.
- `active` : if set true it will activate a listener to the view (default: true).
- `delay` : set the frequency for the listener (default: 200).

##Uage
```js
import Inview from 'react-native-inview'

render() {
  return (
  <ScrollView>
    <Inview onChange={inView => console.log('Inview: '+ inView)}>
      ....
    </Inview>

    <Inview onChange={inView => console.log('Inview: '+ inView)}>
      ....
    </Inview>

  </ScrollView>
  );
}
```
