# Changelog

All notable changes to Transcribo will be documented in this file.

## [0.1.4] - 2026-01-08

### Added
- Multi-language transcription support with 20 common languages (English default)
- New "Advanced" settings tab for speech-to-text model configuration
- Support for all Whisper model variants (tiny, base, small, medium, large-v2, large-v3, distil variants)
- Auto-Detect language option with latency warning

### Changed
- Transcription language is now configurable in General settings
- Model selection moved from hardcoded to user-configurable in Advanced settings
- Model loading now uses local cache first (faster startup, works offline)
- Removed transcription text from logs (still saved to history)

---

## [0.1.3] - 2026-01-06

### Added
- Floating widget now enabled by default for new users
- System sleep/wake detection with automatic hotkey re-registration
- Improved help text in LLM settings explaining test connection behavior
- Edit and Delete buttons for user-created custom modes in Settings

### Fixed
- Hotkey stops working after computer wakes from sleep/hibernate (increased re-registration delay to 2s with additional stabilization delays)
- Floating widget briefly showing previous state (e.g., cyan LLM) before switching to correct state on new recording
- Settings window could not be resized horizontally due to long LLM help text

### Changed
- Updated mode description text to clarify LLM requirements for non-default modes
- Improved startup tray message to guide users to the icon location and mention the hotkey
- Simplified preset modes: "DeepNote" → "Notes", "MailPolisher" → "Email", "ChatFlow" → "Chat"
- Removed "Texter" mode (functionality merged into expanded "Chat" mode)
- Enhanced "Chat" mode to support Twitter, Discord, and other social platforms
- Enhanced all preset system prompts with detailed formatting instructions
- Increased default LLM request timeout from 30s to 120s

---

## [0.1.2] - 2026-01-06

### Added
- Splash screen during application startup to improve perceived load time
- New transparent logo branding
- Window icons for Settings and History windows

### Fixed
- Settings window crash on open (UI initialization restored)
- Test Connection button crash in LLM settings
- Application unexpectedly exiting when closing Settings window
- Custom Mode help button tooltip readability (black text on white background)

### Changed
- LLM connection error messages now more descriptive
- Mode names and prompts refined

---

## [0.1.1] - 2026-01-05

### Added
- Voice Activity Detection (VAD) for hands-free recording
- Floating status widget with draggable UI
- History window with search and copy functionality
- Multiple transcription modes (Raw, Clean, Formal, Custom)
- LLM integration for text post-processing
- Auto-paste feature

### Fixed
- Various UI alignment issues
- History copy feedback improvements

---

## [0.1.0] - 2026-01-04

### Added
- Initial release
- Global hotkey (Ctrl+Space) for push-to-talk recording
- OpenAI Whisper-based local transcription
- System tray integration
- Automatic clipboard copy of transcriptions
- Settings persistence
