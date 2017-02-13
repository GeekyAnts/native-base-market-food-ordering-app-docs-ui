# Start Building Your App

[Swiggy App](http://market.nativebase.io/view/react-native-swiggy-app-theme) guides you throughout building your app, providing the steps and procedure to customize.


**Contents discussed in this section:**
* [How to add new Component?](#new-component)
* [How to add new StyleSheet?](#new-styleSheet)

<a id="new-component"></a>
### How to add new component

* Create a new folder, say ``` newComponent ``` and place it under ``` /js/src``` .
* Create a new file ``` index.js``` , within this folder.
* Name the class same as that of folder name.

```
class NewComponent extends Component {
    ...
}
```

<a id="new-stylesheet"></a>
### How to add new styleSheet

Create a new file ``` styles.js``` , place it under ```/js/src/newComponent```.

```import``` newly created StyleSheet into the Component.
```
import styles from './styles';
class NewComponent extends Component {
    ...
}
```
