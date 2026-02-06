# AI Quest Game - AI & Testing

A comprehensive interactive quiz game designed to test knowledge in artificial intelligence and software testing. Features 9 progressive levels with 45+ questions, real-time scoring, and Google Sheets integration for result tracking.

## 🎮 Features

✅ **9 Progressive Levels** with 45+ carefully crafted questions
✅ **Orange Theme Design** with modern, responsive UI
✅ **Built-in Debug Console** for development and troubleshooting  
✅ **Tab Switch Protection** to prevent cheating during gameplay
✅ **Google Sheets Integration** for automatic result logging
✅ **30-Minute Timer** with real-time countdown
✅ **Multiple Question Types** - Multiple choice and open-ended
✅ **Real-time Scoring** with immediate feedback
✅ **Session Tracking** with unique session IDs
✅ **User Information Collection** (name, project, role)
✅ **Anti-cheat Features** including tab monitoring

## 📋 Game Levels

1. **AI Fundamentals** - Basic AI concepts and terminology
2. **Machine Learning Basics** - Core ML principles and algorithms
3. **Testing Fundamentals** - Software testing principles
4. **AI Testing Strategies** - Specialized testing for AI systems
5. **Advanced AI Concepts** - Deep learning and neural networks
6. **Testing Tools & Frameworks** - Popular testing tools and methodologies
7. **AI Ethics & Bias** - Ethical considerations in AI development
8. **Performance Testing** - AI system performance evaluation
9. **Future of AI & Testing** - Emerging trends and technologies

## 🚀 Quick Start

1. **Open the Game**: Open `index.html` in a web browser
2. **Enter Details**: Provide your name, project, and role
3. **Start Playing**: Begin with Level 1 and progress through all 9 levels
4. **View Results**: All responses are automatically saved to Google Sheets

## 🔧 Technical Setup

### Local Development
```bash
# Start a local HTTP server (Python)
python -m http.server 8000

# Or using Node.js
npx http-server

# Access the game at http://localhost:8000
```

### Google Sheets Integration

The game automatically saves all test results to Google Sheets with the following data:
- Timestamp
- User information (name, project, role)
- Level and question details
- Answers and scoring
- Session tracking
- Tab switch monitoring

**Sheet Name**: `AI_Testing_Results`
**Deployment URL**: `https://script.google.com/macros/s/AKfycbwTZgR1n99uVvJHLHDRlDO_W0temDe0NVQxUUKdeKauCJmKHzcodeUFn5VU2jKoGYTfMA/exec`

## 📁 Project Structure

```
AI-Quest/
├── index.html              # Main game interface
├── google-apps-script.js   # Google Apps Script for sheets integration
├── sd-global-logo.png      # Logo image
└── README.md              # This documentation
```

## 🎯 Game Features

### Scoring System
- **Multiple Choice**: 10 points per correct answer
- **Open-ended**: 15 points per valid response
- **Real-time feedback** with immediate score updates

### Anti-Cheat Protection
- Tab switch detection and counting
- Session-based tracking
- Automatic violation reporting

### Debug Console
Press `Ctrl+Shift+D` to toggle the debug console for:
- Real-time logging
- Session information
- Performance monitoring
- Error tracking

## 🛠️ Configuration

### Google Apps Script Setup
1. Create a new Google Apps Script project
2. Copy code from `google-apps-script.js`
3. Deploy as web app with execute permissions for "Anyone"
4. Update the `GOOGLE_SCRIPT_URL` in `index.html`

### Customization
- **Timer Duration**: Modify the timer value in JavaScript
- **Questions**: Add/edit questions in the `levels` array
- **Styling**: Update CSS variables in the `<style>` section
- **Scoring**: Adjust point values in the `submitAnswer()` function

## 📊 Data Collection

All game sessions collect:
- User demographics and role information
- Question-by-question responses and timing
- Tab switching behavior and violations
- Final scores and completion status
- Unique session identifiers for tracking

## 🔒 Privacy & Security

- No personal data beyond name and role is collected
- All data is stored in designated Google Sheets
- Session IDs are randomly generated
- No tracking cookies or persistent storage

## 🐛 Troubleshooting

### Common Issues
- **Google Sheets not saving**: Check deployment URL and permissions
- **Timer not working**: Ensure JavaScript is enabled
- **Questions not loading**: Verify HTML file structure
- **Debug console issues**: Use Ctrl+Shift+D to toggle

### Debug Information
The game includes comprehensive logging accessible via the debug console for troubleshooting connectivity and functionality issues.

## 📝 License

This project is for educational and assessment purposes. Please ensure proper attribution when using or modifying the code.

---

*Last updated: February 6, 2026*
