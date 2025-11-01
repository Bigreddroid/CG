# CreatorGuard Installation Guide

## Prerequisites

Before you can run CreatorGuard, you need to install Node.js and npm.

### Step 1: Install Node.js

1. **Download Node.js:**
   - Visit: https://nodejs.org/
   - Download the LTS (Long Term Support) version (recommended: v18 or v20)
   - Run the installer and follow the setup wizard
   - Make sure to check "Add to PATH" during installation

2. **Verify Installation:**
   Open PowerShell or Command Prompt and run:
   ```bash
   node --version
   npm --version
   ```
   You should see version numbers for both commands.

### Step 2: Install Project Dependencies

Once Node.js is installed, navigate to the project directory and install dependencies:

```bash
cd creatorguard
npm install
```

This will install all required packages including:
- React 18
- React Router
- Tailwind CSS
- Recharts
- Lucide React Icons

### Step 3: Start the Development Server

```bash
npm start
```

The app will:
- Start on http://localhost:3000
- Automatically open in your browser
- Hot reload when you make changes

### Step 4: Login

Use these credentials to access the dashboard:
- **Email:** `creator.elite@example.com`
- **Password:** `password123`

## Troubleshooting

### Port 3000 Already in Use
If you get an error that port 3000 is in use:
```bash
set PORT=3001 && npm start
```

### npm Install Fails
Try clearing cache and reinstalling:
```bash
npm cache clean --force
rm -rf node_modules package-lock.json
npm install
```

### Windows PowerShell Issues
If you encounter permission errors, run PowerShell as Administrator.

## Build for Production

When ready to deploy:
```bash
npm run build
```

This creates an optimized production build in the `build/` folder.

## Next Steps

After the app is running:
1. ✅ Explore all pages and features
2. ✅ Test mobile responsiveness
3. ✅ Connect to your backend API
4. ✅ Integrate real authentication
5. ✅ Add watermarking functionality
6. ✅ Connect blockchain smart contracts

Your CreatorGuard app is ready to go! 🚀

