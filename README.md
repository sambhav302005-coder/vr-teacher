# VR Teacher - AI-Powered Virtual Learning Platform

An immersive VR education application that integrates Convai conversational AI with Ready Player Me avatars to create interactive virtual classroom experiences.

## 🎯 Features

- **AI-Powered Conversations**: Natural language processing powered by Convai API
- **Realistic Avatars**: Integration with Ready Player Me for customizable teacher avatars
- **Speech Recognition**: Real-time voice interaction with virtual teachers
- **Immersive VR Experience**: Full VR support for an engaging learning environment
- **Interactive Classroom**: Virtual classroom setting with 3D objects and interactive elements

## 🛠️ Technologies Used

- **Unity 3D** (Version 2021.3 LTS or higher recommended)
- **C#** for scripting
- **Convai API** for conversational AI
- **Ready Player Me SDK** for avatar generation
- **XR Interaction Toolkit** for VR interactions
- **Speech Recognition APIs**

## 📋 Prerequisites

Before you begin, ensure you have the following installed:

- Unity Hub and Unity Editor (2021.3 LTS or newer)
- Git
- VR headset (Meta Quest, HTC Vive, or compatible device)
- Convai API key ([Get one here](https://convai.com))
- Ready Player Me account

## 🚀 Installation

### 1. Clone the Repository

```bash
git clone https://github.com/sambhav302005-coder/vr-teacher.git
cd vr-teacher
```

### 2. Open in Unity

1. Open Unity Hub
2. Click "Add" and select the cloned project folder
3. Open the project (Unity will import all assets)

### 3. Install Required Packages

The project uses Unity Package Manager. These packages should auto-install, but verify:

- XR Interaction Toolkit
- XR Plugin Management
- TextMeshPro
- Ready Player Me SDK
- Convai SDK

To manually install:
1. Open `Window > Package Manager`
2. Click `+` and select "Add package from git URL"
3. Add required packages

### 4. Configure API Keys

1. Create a `Config` folder in `Assets/Resources/` if it doesn't exist
2. Create `APIConfig.cs` or add your keys to the configuration scriptable object:

```csharp
// Example configuration
public class APIConfig : ScriptableObject
{
    public string convaiAPIKey = "YOUR_CONVAI_API_KEY";
    public string readyPlayerMeAppId = "YOUR_RPM_APP_ID";
}
```

3. Never commit API keys to the repository (add to `.gitignore`)

### 5. Setup VR

1. Go to `Edit > Project Settings > XR Plug-in Management`
2. Enable your VR platform (Oculus, OpenXR, etc.)
3. Configure XR settings for your target device

## 📁 Project Structure

```
Assets/
├── Scenes/
│   ├── MainMenu.unity
│   ├── VirtualClassroom.unity
│   └── CalibrationScene.unity
├── Scripts/
│   ├── AI/
│   │   ├── ConvaiManager.cs
│   │   └── SpeechRecognition.cs
│   ├── Avatar/
│   │   ├── AvatarLoader.cs
│   │   └── AvatarAnimationController.cs
│   ├── VR/
│   │   ├── VRController.cs
│   │   └── InteractionHandler.cs
│   └── UI/
│       └── MenuController.cs
├── Prefabs/
│   ├── Teacher Avatar/
│   ├── VR Rig/
│   └── Classroom Objects/
├── Materials/
├── Animations/
└── Resources/
    └── Config/
```

## 🎮 How to Use

### For Developers

1. Open the `MainMenu` scene
2. Press Play in Unity Editor (VR device must be connected)
3. Use the VR controllers to navigate and interact
4. Speak to engage with the AI teacher

### Building for VR Headset

1. Go to `File > Build Settings`
2. Select your target platform (Android for Quest, Windows for PC VR)
3. Click "Build" or "Build and Run"
4. Follow platform-specific deployment instructions

## 🔧 Configuration

### Convai Setup

1. Get your API key from [Convai Dashboard](https://convai.com)
2. Create a character in Convai with appropriate personality and knowledge
3. Copy the Character ID
4. Add both API key and Character ID to your configuration

### Ready Player Me Setup

1. Visit [Ready Player Me Developer Portal](https://readyplayer.me)
2. Create an application and get your App ID
3. Configure avatar customization options
4. Add App ID to configuration

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👥 Authors

- **Sambhav Jain** - [GitHub](https://github.com/sambhav302005-coder) | [LinkedIn](https://www.linkedin.com/in/sambhavjain~/)

## 🙏 Acknowledgments

- Convai for the conversational AI platform
- Ready Player Me for avatar technology
- Unity Technologies for the game engine
- XR Interaction Toolkit community

## 📞 Contact

For questions or support, please open an issue or contact:
- Email: sambhav302005@gmail.com
- LinkedIn: [Sambhav Jain](https://www.linkedin.com/in/sambhavjain~/)

## 🗺️ Roadmap

- [ ] Multi-language support
- [ ] Multiple subject modules (Math, Science, History)
- [ ] Student progress tracking
- [ ] Multiplayer classroom sessions
- [ ] Hand tracking support
- [ ] Mobile VR optimization

---

**Note**: This is an educational project. Please ensure you comply with all API terms of service and data privacy regulations when deploying.
