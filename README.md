# Professor Gong's English Grammar Assistant
龚教授英语语法助手

## Deployment Instructions for Netlify

### Step 1: Prepare Your Files
You need these files:
- `index.html` (main app file)
- `netlify.toml` (configuration)
- `package.json` (dependencies)
- `netlify/functions/chat.js` (API handler)

### Step 2: Deploy to Netlify

#### Option A: Drag & Drop (Recommended)
1. Create a folder on your computer
2. Put all the files in it (maintaining the netlify/functions folder structure)
3. Go to https://app.netlify.com/drop
4. Drag the entire folder into the drop zone

#### Option B: GitHub/Git
1. Push all files to a GitHub repository
2. Connect your repository to Netlify
3. Netlify will auto-deploy

### Step 3: Add Your Anthropic API Key
**IMPORTANT**: After deployment, you MUST add your API key:

1. Go to your Netlify site dashboard
2. Click "Site configuration" → "Environment variables"
3. Click "Add a variable"
4. Add:
   - Key: `ANTHROPIC_API_KEY`
   - Value: Your Anthropic API key (get it from https://console.anthropic.com/)
5. Click "Save"
6. Redeploy your site (Deploy → Trigger deploy → Deploy site)

### Step 4: Test Your App
- Visit your Netlify URL
- Try asking a grammar question
- Audio should work automatically

## Features
- ✅ Bilingual (English/Chinese)
- ✅ AI-powered grammar explanations
- ✅ Text-to-speech (American English male, Chinese female)
- ✅ Topic quick-start cards
- ✅ Secure API handling

## Troubleshooting
- **"API key not configured" error**: Add your ANTHROPIC_API_KEY in environment variables
- **Connection error**: Check that the Netlify Function deployed correctly
- **No audio**: Check browser audio permissions

## System Requirements
- Modern web browser (Chrome, Firefox, Safari, Edge)
- Internet connection
- Valid Anthropic API key

---
Created for English language learners 🎓
