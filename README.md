# **Eloqi** - Professional Audio & Media Suite for macOS

<div align="center">

![Eloqi Logo](https://github.com/user-attachments/assets/c61f6b74-dc6c-4a0d-9f65-aef1bb14ca9c)

**Transform your audio and media workflow with AI-powered professional tools**

[![macOS](https://img.shields.io/badge/macOS-13.0+-blue.svg)](https://www.apple.com/macos/)
[![Swift](https://img.shields.io/badge/Swift-5.0+-orange.svg)](https://swift.org/)
[![License](https://img.shields.io/badge/License-Commercial-green.svg)](LICENSE)
[![Version](https://img.shields.io/badge/Version-1.0-brightgreen.svg)](https://pub-0c627237fa784b5baec2d7b5d777c96a.r2.dev/releases/Eloqi-v1.0.0.dmg)

<a href="https://github.com/itsabhishekolkha/Eloqi/releases/download/v1.0.0/RetinaScale.2.0.0.dmg"><img src="https://github.com/user-attachments/assets/a959a0d3-703f-4740-a6ec-ddbaceb0cf74" width="180" alt="Download for macOS"/></a><br/> 
<sub><b>The latest app version requires macOS 13.0 (Vantura) or later.</b></sub>

</div>
**Note:-** please read the installation guide below for proper guide and details.
---

## ✨ **What Makes Eloqi Special?**

Eloqi combines **cutting-edge technology** with native macOS performance to deliver professional-grade audio and media processing. Built with advanced machine learning models and optimized for Apple Silicon and intel Mac, it's the complete solution for content creators, podcasters, and media professionals.

### 🎯 **Three Powerful Modes**

| **🎤 Text To Speech** | **🔊 Clear Voice AI** | **🛠️ Media Tools** |
|:---:|:---:|:---:|
| Neural text-to-speech with natural voices | AI-powered audio enhancement using state-of-the-art models | 25+ professional media processing tools |
| Multiple languages & voice models | Advanced noise reduction & speech separation | Video, audio, and image conversion |
| ONNX-optimized voice synthesis | Batch processing capabilities(Currently in some Media Tools as of now) |

---

## 🚀 **Advanced AI Features**
 Note:- AI features only for ClearVoice

### 🎙️ ** Neural TTS Engine**
- **High-fidelity voice synthesis** using ONNX neural models
- **Multi-language support** with downloadable voice packs
- **Quality tiers** (low, medium, high) for different use cases
- **Local processing** - no internet required after voice download
- **Custom output directories** with organized file management
- **UUID-based file naming** prevents conflicts
- **Can generate long audio files(Tested 30 min+ audio generation from text currently.)

### 🔥 **ClearVoice - State-of-the-Art Audio AI**

**Advanced Model Selection:**
- **MossFormer2 SE 48K** - Premium speech enhancement at 48kHz
- **MossFormerGAN SE 16K** - GAN-based enhancement for 16kHz audio
- **FRCRN SE 16K** - Fast real-time enhancement
- **MossFormer2 SS 16K** - Advanced speech separation
- **MossFormer2 SR 48K** - AI super-resolution upsampling

**Professional Processing:**
- **Multi-task AI models** for different audio scenarios
- **Real-time progress tracking** with tqdm-style feedback
- **Automatic disk space management** (1GB minimum requirement)
- **Robust error handling** with detailed logging

### 🎬 **Comprehensive Media Tools Suite**
Transform any media file with **25+ professional tools**:

#### 🎵 **Audio Processing**
- **Format Conversion** (MP3, WAV, AAC, FLAC, etc.)
- **Audio Extraction** from videos
- **Speed & Pitch Adjustment**
- **Volume Normalization & Effects**
- **Channel Manipulation** (Stereo/Mono)
- **Audio Trimming & Merging**

#### 🎥 **Video Processing**
- **Format Conversion** (MP4, AVI, MKV, MOV, etc.)
- **Video Compression** with H.264/H.265
- **Resolution Scaling & Custom Sizing**
- **Frame Rate Adjustment**
- **Video Stabilization**
- **Rotation & Flipping**
- **Thumbnail Generation**

#### 🖼️ **Image & Subtitle Tools**
- **Image Format Conversion** & Compression
- **Subtitle Extraction & Embedding**
- **Cover Image Addition**
- **Metadata Viewing & Editing**

---

## 💡 **Technical Excellence**

### ⚡ **Optimized Performance**
- **Native Swift/SwiftUI** implementation for maximum macOS integration
- **Apple Silicon optimization** with only CPU acceleration
       (ClearVoice currently supports WAV files only. To convert other file types to WAV, use the Audio Conversion option in the Tools section. Audio conversion will produce the highest quality possible, resulting in larger file sizes, which may increase ClearVoice processing time as files are generated using CPU only, why???, Well CUDA is not supported on macOS because it requires NVIDIA GPUs (available on Linux/Windows) so Mac os will use CPU only.)
- **Efficient memory management** for large audio files
- **Asynchronous processing** with real-time progress updates
- **Background task handling** with proper resource cleanup


### 🔒 **Privacy & Security**
- **100% local processing** - your audio never leaves your device
- **No telemetry or data collection** - complete privacy
- **Sandboxed execution** with proper macOS security integration
- **Temporary file cleanup** - automatic resource management
- **Application Support integration** for proper macOS file organization

---

## 🎯 **Perfect For**

| **Content Creators** | **Podcasters** | **Video Editors** |
|:---:|:---:|:---:|
| AI voice generation | Professional audio cleanup | Format compatibility | 
| Quick media conversion | Noise reduction & enhancement | Batch processing | 
| Thumbnail generation | Speech separation | Resolution scaling |

---

## 📱 **System Requirements**

### **Minimum Requirements**
- **macOS 13.0** or later
- **4GB RAM** (8GB recommended for AI processing)
- **2GB** available storage space
- **Intel or Apple Silicon** processor

### **Recommended for AI Features**
- **macOS 13.0** or later
- **Apple Silicon (M1/M2/M3)** for optimal AI performance
- **8GB RAM** or higher
- **Metal-compatible GPU** for acceleration
- **SSD storage** for faster model loading

### **Storage Requirements**
- **Base app**: ~3.62GB
- **Voice models**: 50-200MB per voice
- **AI models**: Included in app bundle
- **Working space**: 1GB minimum free space required

---

## 🚀 **Quick Start**

## Installation

### Download and Install
1. Download the latest release from [GitHub Releases](https://pub-0c627237fa784b5baec2d7b5d777c96a.r2.dev/releases/Eloqi-v1.0.0.dmg)
2. Drag Eloqi to your Applications folder to complete the installation

### Important Security Notice for macOS Users

When you first attempt to open Eloqi, macOS may display a warning message stating that the app "cannot be opened because it is from an unidentified developer" or that it "may damage your computer." **This is a normal security response and does not indicate any actual threat.**

#### Why This Happens
As an independent student developer, I currently don't have an Apple Developer License, which means:
- The app is not code-signed with Apple's official developer certificate
- The app has not been notarized through Apple's automated security review process
- macOS Gatekeeper treats unsigned applications as potentially unsafe by default

This is a standard security measure Apple implements for all unsigned applications, regardless of their actual safety.

#### How to Open Eloqi Safely

**Method 1: Using Terminal (Recommended)**
```bash
sudo xattr -rd com.apple.quarantine /Applications/Eloqi.app
```
This command removes the quarantine flag that prevents the app from opening. After running this command, Eloqi will launch normally.

**Method 2: System Preferences**
1. Go to System Preferences → Security & Privacy
2. Click "Open Anyway" when the blocked app notification appears
3. Confirm your choice when prompted

#### Future Plans
I am working toward obtaining proper code signing certificates to eliminate this security warning in future releases. Thank you for your understanding as I continue developing Eloqi as a student project.

---

*If you encounter any issues during installation, please [open an issue](https://github.com/yourusername/eloqi/issues) on GitHub.*
4. **First launch** - macOS will verify the app signature
5. **Grant permissions** for file access when prompted

### **Getting Started with Eloqi**

#### **Text-to-Speech (Piper TTS)**
1. Select your preferred voice and quality level
2. Download voice models from settings(one-time setup per voice)
   Note: There is a bug in the app that when user downloads any voice it doesn't appear in downloaded voices instantly to resolve this after downloading voices close settings and reopen, that's it voices are now appears as downloaded.
4. Enter your text and choose output location
5. Generate high-quality speech audio

#### **ClearVoice Enhancement**
1. Choose the appropriate AI model for your audio type
2. Select input audio file (supports most formats)
3. Pick enhancement task (noise reduction, separation, etc.)
4. Watch real-time progress as AI processes your audio

### 💡 **Pro Tips**
- **Voice Models**: Download multiple voices for different projects
- **AI Models**: MossFormer2 models offer the best quality for most use cases
- **Batch Processing**: Use Media Tools for processing multiple files
- **Performance**: Apple Silicon Macs provide 2-3x faster AI processing(only with CPU)

---

##  **Screenshots**

<div align="center">

### Neural Text-to-Speech
![TTS Interface](https://github.com/user-attachments/assets/18eb8ee4-b9d3-49b2-9f40-078f783fd3f6)


### ClearVoice AI Enhancement
![ClearVoice](https://github.com/user-attachments/assets/f4d1ef94-8a3c-494c-b326-d2c25f27f24c)

### Comprehensive Media Tools
![Media Tools 1](https://github.com/user-attachments/assets/d66e25b1-ce8b-418d-98f2-98ffd17515fd)
![Media Tools 2](https://github.com/user-attachments/assets/3913c935-4cbd-4735-bf59-cdfb42624462)
![Media Tools 3](https://github.com/user-attachments/assets/fd21fbb9-853e-4627-9c8d-7a7161ad692d)


</div>

---

##  **Technical Architecture**

- **SwiftUI** for native macOS experience
- **AVFoundation** for professional audio processing
- **Core ML** for Apple's machine learning integration
- **ONNX Runtime** for cross-platform AI model support
- **Metal** for GPU acceleration
- **Speech Framework** for voice recognition
- **Piper TTS Engine** for neural speech synthesis
- **MossFormer/FRCRN Models** for audio enhancement

**Model Details:**
- **ONNX format** for optimal performance and compatibility
- **Quantized models** for efficient memory usage
- **Dynamic loading** - models loaded only when needed
- **Progressive processing** with real-time feedback
- **Error recovery** - Proper handling of processing failures

---

## 📈 **Roadmap & AI Enhancements**

### **Coming Soon**
- [ ] **Real-time voice cloning** with few-shot learning
- [ ] **Batch TTS processing** for large documents
- [ ] **More Natural Voices** for TTS
---

## 🤝 **Support & Community**
- If you find *Eloqi* useful, consider **giving** it **a star** to make it more visible.
- If you find my work useful, please consider Give me a **Star** and follow me on **GitHub**:heart:

Got questions, issues, or ideas bout what we can impliment? Want to help Eloqi grow? Here's how to connect:

- **📧 Email Support**: [support@eloqi.com](mailto:Abhishekolkha555@gmail.com)
- **🐛 Bug Reports**: [GitHub Issues](https://github.com/itsabhishekolkha/Eloqi/issues)
- **💡 Feature Requests**: [GitHub Discussions](https://github.com/itsabhishekolkha/Eloqi/discussions)

---

## 💰 **Pricing**

<div align="center">

**Support Eloqi Development - Choose Your Payment Method**

[💳 **Razorpay**](https://rzp.io/rzp/Eloqi) • [🌍 **PayPal**](https://www.paypal.com/ncp/payment/QKC9JKXXANTMC) • [☕ **Buy Me a Coffee**](https://buymeacoffee.com/abhishekolkha)

[🛒 **Get Pro License - 75% OFF**](https://github.com/itsabhishekolkha/Eloqi/releases) • [🆓 **Download Trial**](https://pub-0c627237fa784b5baec2d7b5d777c96a.r2.dev/releases/Eloqi-v1.0.0.dmg)

**🔒 30-day money-back guarantee • 🎯 One-time purchase, no subscriptions • 🚀 Instant access to everything**

</div>

---

## 🌟 **Model Performance**
*Results may vary based on hardware configuration and audio content*

## Credits
We are deeply grateful to the open-source community for their remarkable contributions, which have been pivotal in the development of this project. Special recognition goes to the following:

ClearerVoice-Studio by @modelscope. Their cutting-edge AI-powered speech processing toolkit, featuring advanced models for speech enhancement, separation, and super-resolution, forms a critical foundation of our audio processing capabilities. We sincerely appreciate their dedication to advancing speech technology and sharing their pre-trained models and scripts with the community.
Piper by @rhasspy. Their high-performance, local neural text-to-speech system has greatly enriched our project's ability to deliver seamless, high-quality speech synthesis. We are thankful for their innovative approach and commitment to open-source principles.
Contributors: If anyone wants to suggest you are most welcome.
Open-Source Community: This project thrives thanks to the countless open-source libraries and tools we build upon. We are committed to contributing back to this vibrant ecosystem and welcome others to join us in this collaborative journey.


## License
[MIT License](https://github.com/)

 


**Made with ❤️ and AI for macOS • Copyright © 2025 Eloqi**


</div>
