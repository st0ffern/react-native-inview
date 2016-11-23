# react-native-inview
Detects if a element is inside a ScrollView or a ListView and reports back.

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
