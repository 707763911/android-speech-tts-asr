
### 5. `android-speech-tts-asr/README.md`

```markdown
# Android Speech TTS ASR

Android 语音双向工程实现：文字转语音（TTS）与语音转文本（ASR）的统一封装。仓库内不包含客户文本、品牌音色、客户语音或商业语音数据。

## 功能
### 文字转语音（TTS）
- 文本输入与朗读
- 语言/音色选择（取决于系统 TTS 引擎）
- 语速、音调设置
- 播放/暂停/停止与队列管理
- 引擎可用性检测与错误回调

### 语音转文本（ASR）
- 录音权限申请
- 实时/分段语音识别
- 识别结果回调与置信度展示
- 错误处理与重试
- 可选离线 ASR 适配入口

### 统一封装
- TTS/ASR 统一接口与状态管理
- 音频焦点与生命周期处理
- 统一日志与异常回调

## 技术栈
Kotlin、Android TextToSpeech API、Android SpeechRecognizer、可选 Vosk/Whisper（按实际实现）

## 快速开始
1. Android Studio 打开项目
2. 授予麦克风权限，确保设备安装 TTS 引擎
3. 输入文本朗读，或点击录音进行语音识别

## 安全与合规
- 输入文本与音频为脱敏合成数据
- 默认不上传用户音频
- 不包含客户文本、语音数据与商业音色

## License
MIT
