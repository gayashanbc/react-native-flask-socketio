# react-native-flask-socketio

- Clone the repo using ```git cline --recurse-submodules https://github.com/gayashanbc/react-native-flask-socketio.git```
- Navigate to the 'server' folder.
- Make sure that you have the reuired libraries installed and run the command ```python3 chat.py```
- Navigate back to the root folder
- Run ```yarn install``` or ```npm install```
- Make sure you have React Native CLI installed and run ```react-native run-android``` or ```react-native run-ios```

### Notice
Based on your device change the host port accordingly in the App.js file.
```
  constructor(props){
    super(props);
    this.socket = io(`http://10.0.3.2:5000/chat`);

    this.socket.on('connect', () => {
      console.log('connected')
    });
  }
```

#### Genymotion
10.0.3.2

#### Android Studio Emulator
10.0.2.2

#### External device
obtain the IP of your computer. (Computer and the device should be on the same network)
