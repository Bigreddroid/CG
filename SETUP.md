# CreatorGuard Setup Instructions

## Current Status

The CreatorGuard project files have been created successfully. However, **Node.js needs to be installed** before you can run `npm install`.

## Step-by-Step Setup

### 1. Install Node.js (Required First Step)

1. **Download Node.js:**
   - Visit: https://nodejs.org/
   - Click "Download Node.js (LTS)" - This is the recommended version
   - The file will be something like `node-v20.x.x-x64.msi`

2. **Install Node.js:**
   - Run the downloaded installer
   - **IMPORTANT:** Make sure "Add to PATH" is checked during installation
   - Click "Next" through all prompts
   - Click "Install" and wait for completion

3. **Restart Your Terminal:**
   - Close ALL PowerShell/Command Prompt windows
   - Open a NEW PowerShell or Command Prompt window
   - This is required for PATH changes to take effect

4. **Verify Installation:**
   ```bash
   node --version
   npm --version
   ```
   Both commands should show version numbers (e.g., v20.10.0 and 10.2.3)

### 2. Navigate to Project Directory

Open PowerShell/Command Prompt and run:

```bash
cd C:\Users\Varun\creatorguard
```

Or if you're already in your user directory:
```bash
cd creatorguard
```

### 3. Install Dependencies

```bash
npm install
```

This will install all required packages:
- React 18
- React Router
- Tailwind CSS
- Recharts
- Lucide React Icons
- And all their dependencies

**Expected output:** You'll see a progress bar and then "added X packages"

### 4. Start the Development Server

```bash
npm start
```

The app will:
- Start on http://localhost:3000
- Automatically open in your default browser
- Hot reload when you make code changes

### 5. Login to the App

Use these credentials:
- **Email:** `creator.elite@example.com`
- **Password:** `password123`

## Troubleshooting

### "npm is not recognized"
- **Solution:** Node.js is not installed or not in PATH
- **Fix:** Install Node.js from nodejs.org and restart your terminal

### "Cannot find module"
- **Solution:** Dependencies not installed
- **Fix:** Run `npm install` again

### "Port 3000 is already in use"
- **Solution:** Another app is using port 3000
- **Fix:** 
  ```bash
  set PORT=3001
  npm start
  ```

### Installation Takes Too Long
- This is normal for first install
- npm is downloading ~200MB of packages
- Be patient, it usually takes 2-5 minutes

## Project Location

Your project is located at:
```
C:\Users\Varun\creatorguard\
```

If you can't find it, search for `package.json` in File Explorer.

## Next Steps After Installation

1. ✅ Explore the Dashboard
2. ✅ Check out the Leaks page
3. ✅ Test the Evidence modal
4. ✅ Try mobile view (resize browser)
5. ✅ Review the code in `src/` folder

## Build for Production

When ready to deploy:
```bash
npm run build
```

This creates an optimized build in the `build/` folder.

---

**Need Help?** If npm commands still don't work after installing Node.js:
1. Restart your computer (ensures PATH is fully updated)
2. Open a new terminal window
3. Try again

Good luck! 🚀

