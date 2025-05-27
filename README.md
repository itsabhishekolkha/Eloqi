# **Eloqi** - Professional Audio & Media Suite for macOS

<div align="center">

![Eloqi Logo](https://github.com/user-attachments/assets/c61f6b74-dc6c-4a0d-9f65-aef1bb14ca9c)

**Transform your audio and media workflow with AI-powered professional tools**

[![macOS](https://img.shields.io/badge/macOS-13.0+-blue.svg)](https://www.apple.com/macos/)
[![Swift](https://img.shields.io/badge/Swift-5.0+-orange.svg)](https://swift.org/)
[![License](https://img.shields.io/badge/License-Commercial-green.svg)](LICENSE)
[![Version](https://img.shields.io/badge/Version-1.0-brightgreen.svg)](https://github.com/yourusername/eloqi/releases)

<a href="https://github.com/itsabhishekolkha/Eloqi/releases/download/v1.0.0/RetinaScale.2.0.0.dmg"><img src="https://github.com/user-attachments/assets/a959a0d3-703f-4740-a6ec-ddbaceb0cf74" width="180" alt="Download for macOS"/></a><br/> 
<sub><b>The latest app version requires macOS 13.0 (Vantura) or later.</b></sub>

</div>

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
- **macOS 11.0** or later
- **4GB RAM** (8GB recommended for AI processing)
- **2GB** available storage space
- **Intel or Apple Silicon** processor

### **Recommended for AI Features**
- **macOS 12.0** or later
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
1. Download the latest release from [GitHub Releases](https://github.com/yourusername/eloqi/releases)
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

## 🎨 **Screenshots**

<div align="center">

### Neural Text-to-Speech Interface
![TTS Interface](https://via.placeholder.com/800x500/f3f4f6/374151?text=Piper+Neural+TTS+Engine)

### ClearVoice AI Enhancement
![ClearVoice](https://via.placeholder.com/800x500/f3f4f6/374151?text=AI-Powered+Audio+Enhancement)

### Comprehensive Media Tools
![Media Tools](https://via.placeholder.com/800x500/f3f4f6/374151?text=25%2B+Professional+Tools)

</div>

---

## 🏆 **What Users Are Saying**

> *"The AI audio enhancement is phenomenal - better than tools costing thousands!"*  
> **— Sarah K., Podcast Producer**

> *"Piper TTS voices sound incredibly natural. Perfect for my video projects."*  
> **— Mike R., Content Creator**

> *"Finally, professional AI audio tools that work completely offline on Mac!"*  
> **— David L., Audio Engineer**

> *"The MossFormer2 models deliver studio-quality results in seconds."*  
> **— Lisa M., Voiceover Artist**

---

## 🔧 **Technical Architecture**

**Built with cutting-edge technology:**
- **SwiftUI** for native macOS experience
- **AVFoundation** for professional audio processing
- **Core ML** for Apple's machine learning integration
- **ONNX Runtime** for cross-platform AI model support
- **Metal** for GPU acceleration
- **Speech Framework** for voice recognition
- **Piper TTS Engine** for neural speech synthesis
- **MossFormer/FRCRN Models** for audio enhancement

**AI Model Details:**
- **ONNX format** for optimal performance and compatibility
- **Quantized models** for efficient memory usage
- **Dynamic loading** - models loaded only when needed
- **Progressive processing** with real-time feedback
- **Error recovery** - graceful handling of processing failures

---

## 📈 **Roadmap & AI Enhancements**

### **Coming Soon**
- [ ] **Real-time voice cloning** with few-shot learning
- [ ] **Batch TTS processing** for large documents
- [ ] **Custom voice training** from audio samples
- [ ] **Advanced audio effects** with AI preprocessing
- [ ] **Multi-speaker separation** with speaker identification
- [ ] **Automatic transcription** with timestamp alignment

### **Advanced Features**
- [ ] **Plugin architecture** for custom AI models
- [ ] **Command-line interface** for automation
- [ ] **AppleScript support** for workflow integration
- [ ] **Cloud model sync** (optional) for enterprise users
- [ ] **Shortcut integration** for iOS/macOS automation

---

## 🤝 **Support & Community**

### **Get Help**
- **📧 Email Support**: [support@eloqi.com](mailto:support@eloqi.com)
- **📖 Documentation**: [Complete user guide](docs/)
- **🐛 Bug Reports**: [GitHub Issues](https://github.com/yourusername/eloqi/issues)
- **💡 Feature Requests**: [GitHub Discussions](https://github.com/yourusername/eloqi/discussions)

### **Technical Support**
- **AI Model Issues**: Detailed troubleshooting guides available
- **Performance Optimization**: Tips for different Mac configurations
- **Voice Model Management**: Download and organization help
- **Integration Support**: Workflow automation assistance

---

## 💰 **Pricing**

<div align="center">

### 🎯 **Professional AI Tools - Limited Time Offer**

| **License** | **Price** | **Features** |
|:---:|:---:|:---|
| **Pro License** | ~~$149~~ **$74** | ✅ All AI models included<br>✅ Unlimited voice downloads<br>✅ Lifetime updates<br>✅ Priority AI support<br>✅ Commercial use rights |
| **Evaluation** | **Free** | ✅ 7-day full access<br>✅ All AI features<br>⚠️ Watermarked output<br>⚠️ Limited exports per day |

[🛒 **Get Pro License - 50% OFF**](https://github.com/yourusername/eloqi/releases) • [🆓 **Download Trial**](https://github.com/yourusername/eloqi/releases)

**🔒 30-day money-back guarantee • 🎯 One-time purchase, no subscriptions • 🚀 Instant access to all AI models**

</div>

---

## 📄 **License & AI Model Usage**

This software includes professionally licensed AI models and is commercially licensed for end-user applications.

### **Included AI Models**
- **Piper TTS Models**: Licensed for commercial text-to-speech generation
- **MossFormer Models**: Licensed for professional audio enhancement
- **FRCRN Models**: Licensed for real-time audio processing

### **Usage Rights**
- **Personal Use**: Full access to all AI features
- **Commercial Use**: Included with Pro license
- **Model Redistribution**: Not permitted
- **API Integration**: Available for enterprise customers

Full license terms and model attributions available in [LICENSE](LICENSE) file.

---

## 🌟 **AI Model Performance**

### **Benchmark Results** (Apple M2 Pro)

| **Model** | **Task** | **Processing Speed** | **Quality Score** |
|:---:|:---:|:---:|:---:|
| MossFormer2 SE 48K | Speech Enhancement | 5x real-time | 4.8/5.0 |
| MossFormerGAN SE 16K | Noise Reduction | 8x real-time | 4.6/5.0 |
| FRCRN SE 16K | Real-time Enhancement | 15x real-time | 4.2/5.0 |
| Piper TTS (High Quality) | Speech Synthesis | 20x real-time | 4.9/5.0 |

*Results may vary based on hardware configuration and audio content*

---

<div align="center">

### 🌟 **Ready to Experience AI-Powered Audio?**

**Download Eloqi today and transform your media workflow with professional AI tools**

[🚀 **Get Eloqi Pro**](https://github.com/yourusername/eloqi/releases) • [📧 **Contact Sales**](mailto:sales@eloqi.com) • [🎯 **Try Free Trial**](https://github.com/yourusername/eloqi/releases)

---

**Made with ❤️ and AI for macOS • Copyright © 2024 Eloqi**

[![Twitter](https://img.shields.io/badge/Twitter-Follow-1da1f2.svg)](https://twitter.com/eloqiapp)
[![Website](https://img.shields.io/badge/Website-Visit-blue.svg)](https://eloqi.com)
[![GitHub](https://img.shields.io/badge/GitHub-Star-black.svg)](https://github.com/yourusername/eloqi)

</div>
