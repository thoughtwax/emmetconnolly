# Quick AI

**The fastest way to query ChatGPT and Claude simultaneously with voice input.**

## 🚀 Features

- **Voice-First**: Tap the mic button and speak your query
- **Parallel Queries**: Sends your question to ChatGPT and Claude APIs simultaneously
- **Side-by-Side Comparison**: See both responses at once
- **One-Tap Selection**: Tap your preferred response to:
  - Copy the full conversation to clipboard
  - Attempt to open the native app (ChatGPT or Claude)
  - Paste and continue the conversation there
- **Query History**: Automatically saves your last 10 queries locally
- **PWA**: Add to iOS home screen for instant access

## 📱 Setup Instructions

### 1. Get Your API Keys

#### OpenAI (ChatGPT) API Key:
1. Go to [platform.openai.com](https://platform.openai.com/api-keys)
2. Sign in or create an account
3. Click "Create new secret key"
4. Copy the key (starts with `sk-`)
5. Add $5-10 credit to your account

#### Anthropic (Claude) API Key:
1. Go to [console.anthropic.com](https://console.anthropic.com/)
2. Sign in or create an account
3. Go to "API Keys" section
4. Click "Create Key"
5. Copy the key (starts with `sk-ant-`)
6. Add $5-10 credit to your account

**Cost**: Each dual query costs ~$0.01-0.05 (very cheap!)

### 2. Add to iOS Home Screen

1. Open Safari on your iPhone
2. Navigate to: `https://emmetconnolly.com/projects/quick%20AI/index.html`
3. Tap the Share button (square with arrow)
4. Scroll down and tap "Add to Home Screen"
5. Name it "Quick AI" and tap "Add"

### 3. Configure API Keys

1. Open the Quick AI app from your home screen
2. Tap the ⚙️ settings button (top right)
3. Paste your OpenAI API key
4. Paste your Anthropic API key
5. Tap "Save"

**Privacy**: Your API keys are stored locally in your browser and are ONLY sent directly to OpenAI and Anthropic. They never go anywhere else.

## 🎯 How to Use

1. **Launch** the app from your home screen
2. **Tap** the microphone button
3. **Speak** your query
4. **Wait** ~2-3 seconds for both AI responses
5. **Compare** the responses side-by-side
6. **Tap** your preferred response to:
   - Copy it to clipboard
   - Open the native app to continue

## 🔧 Technical Details

- **Frontend**: Vanilla JavaScript (single HTML file)
- **APIs**:
  - OpenAI GPT-4o-mini (fast, cheap)
  - Claude 3.5 Sonnet (latest model)
- **Storage**: IndexedDB for local history
- **Speech**: Web Speech API (built into iOS Safari)
- **PWA**: Full progressive web app support

## 🛠️ Development

The entire app is a single `index.html` file with embedded CSS and JavaScript. To modify:

1. Edit `projects/quick AI/index.html`
2. Refresh in browser
3. Changes apply immediately (no build step!)

## 📝 Notes

- Requires internet connection to query APIs
- Speech recognition requires microphone permissions
- Works best in Safari on iOS
- History is stored locally (not synced across devices)
- URL scheme deep linking is experimental (may not work on all iOS versions)

## 🎨 Customization

Edit the `index.html` file to:
- Change models (GPT-4, Claude Opus, etc.)
- Adjust max_tokens for longer/shorter responses
- Modify colors and styling
- Add more AI services

## 🐛 Troubleshooting

**"Speech recognition not supported"**: Make sure you're using Safari on iOS (not Chrome or Firefox)

**"Please configure API keys"**: Tap the settings button and add your API keys

**"API error 401"**: Your API key is invalid or expired

**"API error 429"**: You've hit rate limits or need to add credits to your account

**Clipboard not working**: Make sure you granted clipboard permissions when prompted

**Native app not opening**: The URL scheme fallback will open the web version instead

## 💡 Future Improvements

- [ ] Support for more AI models (Gemini, etc.)
- [ ] Conversation threading in native apps
- [ ] Export history as JSON/CSV
- [ ] Custom system prompts per AI
- [ ] Offline mode with cached responses

---

Built with ❤️ by Emmet Connolly
