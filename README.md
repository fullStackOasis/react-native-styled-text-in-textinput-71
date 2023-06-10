# react-native-styled-text-in-textinput

This example is based on the default React Native project.

The project was initialized as follows:

`nvm use 14.20.0`

`npx react-native init StyledTextInTextInput71 --version 0.71`

Once the project was created, a few small changes were made. Two `<TextInput>` components were added to demonstrate a bug. (Comment: I just copied the relevant changes from [react-native-styled-text-in-textinput](https://github.com/fullStackOasis/react-native-styled-text-in-textinput) which was a React Native 0.70 project)

The new code is here:

```
    <View style={{paddingHorizontal: 24, borderColor: 'black', borderWidth: 2, margin: 2, borderRadius: 2}}>
    <TextInput multiline>
        <Text style={{"fontWeight":"bold","color":"blue","backgroundColor":"white"}}>David Tabaka</Text>
        <Text> The quick brown fox jumped over the lazy dog</Text>
    </TextInput>
    </View>
    <View style={{paddingHorizontal: 24, borderColor: 'black', borderWidth: 2, margin: 2, borderRadius: 2}}>
    <TextInput multiline>
        <Text style={{"fontWeight":"bold","color":"blue","backgroundColor":"white"}}>David Tabaka</Text>
        <Text> The quick brown fox jumped over the lazy dog and the</Text>
    </TextInput>
    </View>
```

Run the app on an Android device. When the app starts, you will see two `TextInput` components with a thin black border on the screen along with the other default components.

Tap your finger at the very end of the first `TextInput`. Nothing special happens.

Next, tap your finger at the very end of the **second** `TextInput`. You will see the style of the entire content of the `TextInput` change.

This is a bug. The expected behavior is that the style of the content should not change.



https://github.com/fullStackOasis/react-native-styled-text-in-textinput-71/assets/59945095/eb6c4362-e7e6-438e-9ae6-22a74d90d324

