## Firebase SDK support in the Apple Silicon Unity Editor

### Instructions

⚠️ Before proceeding, make sure your project is committed to source control and/or backed up! Proceed at your own risk. 

1. [Download](https://github.com/aroman/firebase-unity-applesilicon/archive/refs/heads/main.zip) this repo
2. In your project, open the directory `Assets/Firebase/Plugins`
3. Copy the `arm64` directory into `Assets/Firebase/Plugins`
4. There should already be a directory named `x86_64` in `Assets/Firebase/Plugins`. Delete it.
5. If your project was already open, you'll need to close and re-open it for the changes to take effect.

### What is this?

If you both:
- Use Unity Editor on an Apple Silicon Mac
- Use the Firebase SDK in your Unity project

...and want to use the Firebase SDK functionality from inside the editor (e.g. Realtime Database)

...you've probably noticed that [this it doesn't work](https://github.com/firebase/quickstart-unity/issues/1100), because the Firebase team has not yet provided a build of the Unity SDK compiled with arm64 Unity Editor support. Fortunately, the Firebase Unity SDK is open source, which allowed me to build the SDK with arm64 Unity Editor support 🎉
