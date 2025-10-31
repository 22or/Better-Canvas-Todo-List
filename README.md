# Better Canvas Todo List

A modern, fast, and organized todo list for Instructure Canvas LMS.

Better Canvas Todo List fetches and displays all your assignments across all courses in one streamlined view, with automatic refreshing and a modern, responsive UI.

## Features

- **Consolidated View**: See todos from each of your courses in one place
- **Modern UI**: Intuitive interface with light and dark mode that's easier on the eyes
- **Fast Loading**: Significantly faster than Canvas's native todo list
- **Auto-Refresh**: Automatically updates every 10 minutes to keep you current
- **Clutter-free**: Organized layout shows assignments and omits announcements, calendar items, etc
- **Supports Delete**: Remove completed items with a single click
- **Universal Compatibility**: Works with any Canvas instance (any university/institution)

## Usage

### Using the Live Site

1. Visit [Better Canvas Todo List](https://22or.github.io/Better-Canvas-Todo-List)

2. Generate a Canvas API token:
   - Log into your Canvas account
   - Navigate to **Account** → **Settings**
   - Scroll to **Approved Integrations**
   - Click **+ New Access Token**
   - Give it a purpose name (e.g., "Better Todo List")
   - Click **Generate Token**
   - Copy the token (you won't be able to see it again!)

3. Enter your Canvas instance URL (e.g., `https://yourschool.instructure.com`)

4. Paste your API token

5. Start managing your assignments!

## Security & Privacy

**Your data never leaves your browser.**

- ✅ All API calls are made directly from your browser to your Canvas instance
- ✅ Your API token is stored locally in your browser only
- ✅ No server-side processing or data collection
- ✅ No third-party services or analytics
- ✅ Open source - verify the code yourself!

**API Token Permissions Required:**
- View todo items
- Delete todo items

*Tip: Tokens can be revoked at any time from your Canvas settings*

## Local Development

**This project comes with a .devcontainer folder and is compatible with GitHub Codespaces.**

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn

### Installation

1. **Clone the repository**
```bash
   git clone https://github.com/22or/Better-Canvas-Todo-List.git
   cd Better-Canvas-Todo-List
```

2. **Install dependencies**
```bash
   npm install
   # or
   yarn install
```

3. **Start the development server**
```bash
   npm start
   # or
   yarn start
```

4. Open [http://localhost:3000](http://localhost:3000) in your browser

### Building for Production
```bash
npm run build
# or
yarn build
```

## Deployment

This is a static React application that can be deployed to any static hosting service:

### GitHub Pages
```bash
npm run deploy
```

### Other Platforms
- **Netlify**: Drag and drop the `build/` folder
- **Vercel**: Connect your GitHub repository
- **AWS S3**: Upload the `build/` folder contents
- **Any static host**: Serve the `build/` directory

## Usage

## Technology Stack

- **Frontend**: React
- **Styling**: BulmaCSS
- **API**: Canvas LMS REST API
- **Build Tool**: Create-React-App
- **Deployment**: Static hosting (GitHub Pages, Netlify, etc.)

## Troubleshooting

### "Invalid API Token" Error
- Verify your token is correct (no extra spaces)
- Check that your token hasn't expired
- Ensure the token has required permissions
- Generate a new token if needed

### Todos Not Loading
- Verify your Canvas URL is correct (include `https://`)
- Check your internet connection
- Ensure you're not behind a restrictive firewall
- Try refreshing your Canvas API token

### Missing Assignments
- Check if assignments are actually in your Canvas todo list
- Some assignment types may not appear in the todo API
- Verify your courses are active and not concluded

### CORS Issues (Development)
- CORS shouldn't be an issue since API calls are made from your browser
- If you encounter CORS errors, check your Canvas instance settings

## Contributing

Contributions are welcome! Here's how to help:

1. **Fork the repository**
2. **Create a feature branch**
```bash
   git checkout -b feature/AmazingFeature
```
3. **Commit your changes**
```bash
   git commit -m 'Add some AmazingFeature'
```
4. **Push to the branch**
```bash
   git push origin feature/AmazingFeature
```
5. **Open a Pull Request**

## Disclaimer

This is an unofficial tool and is not affiliated with, endorsed by, or connected to Instructure or Canvas LMS. Use at your own discretion.

**Made with ❤️ by students, for students**
