# Speech-2-TTS Mod by NocturnalLyfe

Transform your voice chat into hilarious text-to-speech! Uses completely offline speech recognition.

## Features

- Real-time voice -> text -> TTS conversion
- Your actual voice is muted when STT is enabled (only TTS is broadcast)
- Toggle on/off with a single keypress
- Text appears in game chat for all players to see
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
- **F7** - Toggle Speech-to-Text mode ON/OFF

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

No configuration needed! Just press F7 to toggle.

### Using a Better Model (Optional)

For better accuracy, you can replace the model:

1. Download `vosk-model-en-us-0.22` from https://alphacephei.com/vosk/models
2. Extract to `BepInEx/plugins/NocturnalLyfe-Speech2TTS/model/`
3. Update the folder name in the mod code

## Troubleshooting

**Mod not working:**
- Check `BepInEx/LogOutput.log` for errors
- Ensure all DLLs are in the plugin folder
- Verify the model folder exists and is named correctly

**Low accuracy:**
- Speak clearly and at a moderate pace
- Check microphone quality
- Consider using the larger model (vosk-model-en-us-0.22)

**No audio transmission:**
- This is normal when STT is enabled! Your voice is muted and replaced with TTS
- Press F7 to disable STT for normal voice chat

## Technical Details

- **Model**: vosk-model-small-en-us-0.15 (~40MB)
- **Speech Recognition**: Offline Vosk engine
- **Sampling Rate**: 48kHz
- **Language**: English (US)

## Credits

- Mod by Nocturnal
- Vosk Speech Recognition: https://alphacephei.com/vosk/
- BepInEx: https://github.com/BepInEx/BepInEx

## Support

Report issues on GitHub or the Thunderstore page.
https://github.com/NocturnalLyfe/REPO-Speech2TTS

## Changelog

See CHANGELOG.md for version history.