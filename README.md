# Cognigy Chat Client

A professional Node.js REST client for Cognigy.AI with real-time chat benchmarks and analytics.

![Image 1](https://github.com/lalitnayyar/cogignywebchat/blob/main/chrome_DiwkWZMalz.png)
![Image 2](https://github.com/lalitnayyar/cogignywebchat/blob/main/IBNTuEff5s.png)

## Features

- Modern, responsive UI with a professional design
- Real-time chat interface with request/response display
- Live benchmarking sidebar showing:
  - Average response time
  - Total requests
  - Success rate
  - Response time graph
- Built with Express.js and EJS templating
- Uses official Cognigy REST Client

## Installation

1. Clone this repository
2. Install dependencies:
```bash
npm install
```

3. Configure your Cognigy credentials in `src/index.js`:
```javascript
const cognigyOptions = {
    url: process.env.COGNIGY_URL || 'your-endpoint-url',
    userId: process.env.COGNIGY_USER_ID || 'your-user-id',
    // ... other options
};
```

## Running the Application

Start the development server:
```bash
npm run dev
```

Or run in production mode:
```bash
npm start
```

The application will be available at `http://localhost:3000`

## Environment Variables

- `COGNIGY_URL`: Your Cognigy endpoint URL
- `COGNIGY_USER_ID`: Your Cognigy user ID

## Screen Layout Structure

The application features a modern, responsive layout with the following components:

### Main Layout
```
┌─────────────────────────────────────────────────────┐
│                    Chat Section                      │
├─────────────┬───────────────────────────────────────┤
│             │                                       │
│  Analytics  │           Chat Interface              │
│  Sidebar    │                                       │
│             │                                       │
│             │                                       │
└─────────────┴───────────────────────────────────────┘
```

### Analytics Sidebar (Left)
- **Header**
  - Title with icon
  - Refresh button
- **Metric Grid**
  - Response Time
  - Total Tokens
  - Conversations
  - Accuracy Rate
- **Token Usage Chart**
  - Area chart showing prompt/completion tokens
  - Interactive legend
- **Performance Metrics**
  - Memory Usage
  - CPU Load
  - Network Status

### Chat Interface (Right)
- **Header**
  - AI Assistant title
  - Status indicator
- **Chat Container**
  - Message history
  - User/AI messages
  - Code blocks with syntax highlighting
- **Input Area**
  - Message input field
  - Send button with icon

### Responsive Design
- **Desktop**: Full two-column layout
- **Tablet**: Reduced sidebar width
- **Mobile**: 
  - Single column layout
  - Stacked components
  - Optimized for touch

### Key Features
- Glassmorphism design
- Neon accents and gradients
- Real-time analytics
- Collapsible panels
- Smooth animations
- Custom scrollbars

### Theme Variables
```css
:root {
  --sidebar-width: 320px
  --container-padding: 15px
  --border-radius: 12px
  --primary-color: rgb(0, 255, 242)
  --secondary-color: rgb(112, 0, 255)
}
```

### Browser Compatibility
- Modern browsers (Chrome, Firefox, Safari, Edge)
- Responsive from 320px to 1920px+ screens
- Touch-enabled for mobile/tablet devices

## GitHub Commands

### First Time Setup
```bash
# Initialize repository
git init

# Add all files
git add .

# Commit changes
git commit -m "Initial commit"

# Connect to GitHub repository
git remote add origin https://github.com/lalitnayyar/cogignywebchat.git
git branch -M main
git push -u origin main
```

### Regular Updates
```bash
# Check status
git status

# Add new/modified files
git add .

# Commit changes
git commit -m "Your commit message"

# Push to GitHub
git push origin main
```

### Other Useful Commands
```bash
# Pull latest changes
git pull origin main

# View commit history
git log

# Create and switch to new branch
git checkout -b branch-name

# Switch branches
git checkout branch-name

# Merge branches
git merge branch-name
```

## License

MIT

https://github.com/lalitnayyar/cogignywebchat.git
