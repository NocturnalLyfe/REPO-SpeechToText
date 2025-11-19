# Speech-2-TTS Mod by NocturnalLyfe

Transform your voice chat into hilarious text-to-speech! Uses completely offline speech recognition.

## Features

- Real-time voice -> text -> TTS conversion
- Your actual voice is muted when STT is enabled (only TTS is broadcast)
- Toggle on/off with a single keypress -> F8
- TTS speaks in game for all players to hear
- Flexible model support - allowing change to different Vosk Models
- No performance impact

## Installation

### Automatic (Mod Manager)
1. Install via Thunderstore Mod Manager or r2modman
2. Launch the game

### Manual
1. Install BepInEx if not already installed
2. Extract the mod folder to `REPO/BepInEx/plugins/`
3. Launch the game

## Usage

### Controls
- **F7** - Toggle Speech-to-Text Menu Panel
- **F8** - Toggle Speech-to-Text mode ON/OFF Directly

### Modes

**STT Enabled (Default):**
- Your voice is converted to text
- Text is broadcast via in-game chat as TTS
- Your actual voice is muted (others only hear TTS)
- Perfect for robot voice fun!

**STT Disabled:**
- Normal voice chat
- Your real voice is transmitted
- No text-to-speech conversion

## How It Works

1. Speak into your microphone
2. Vosk speech recognition transcribes your voice
3. Text is sent to the game's chat system
4. Game's TTS speaks your message to all players
5. Everyone sees and hears your transcribed speech!

## Configuration

- Toggle Mod On and Off in Menu or F8
- Toggle Model being used ingame or in config.
- Toggle Sensitivity of your voice to the model.
- Toggle Pre-roll capture for better capturing of speech before talking to get full sentences.

### Recommended Models

1. **vosk-model-small-en-us-0.15 (Default)** (~40MB) - Default, fastest, good accuracy
2. **vosk-model-en-us-0.22** (~1.8GB) - Better accuracy, slower
3. **vosk-model-en-us-0.42-gigaspeech** (~2.3GB) - Best accuracy, slowest

#### To Use a Different Model:

1. Download your preferred model from https://alphacephei.com/vosk/models
2. Extract to `BepInEx/plugins/NocturnalLyfe-Speech2TTS/model/`
3. Keep the original folder name (don't rename it)
4. The mod will automatically detect and use it!

**Tip:** You can have multiple models installed - the mod will let you select which one you want to use ingame.

**Warning:** Changing to larger models will take some time depending on the size and your device. Only recommended for stronger devices.

## Troubleshooting

**Mod not working:**
- Check `BepInEx/LogOutput.log` for errors
- Ensure all DLLs are in the plugin folder (libvosk.dll, libgcc_s_seh-1.dll, libstdc++-6.dll, libwinpthread-1.dll)
- Verify at least one model folder exists in the `model/` directory

**Low accuracy:**
- Speak clearly and at a moderate pace
- Check microphone quality
- Consider downloading and changing to vosk-model-en-us-0.22 or vosk-model-en-us-0.42-gigaspeech for better accuracy

**No audio transmission:**
- This is normal when STT is enabled! Your voice is muted and replaced with TTS
- Press F7 to disable STT for normal voice chat

## Technical Details

- **Default Model**: vosk-model-small-en-us-0.15 (~40MB)
- **Speech Recognition**: Offline Vosk engine
- **Sampling Rate**: 48kHz
- **Language**: English (US)
- **Supported Models**: Any Vosk English model compatible with the API

## Credits

- Mod by NocturnalLyfe
- Vosk Speech Recognition: https://alphacephei.com/vosk/
- BepInEx: https://github.com/BepInEx/BepInEx

## Support

Report issues on Discord: Username is Nocturnal0.
https://discord.gg/vPJtKhYAFe

## Changelog

See CHANGELOG.md for version history.