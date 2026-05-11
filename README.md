# HaCham - Jewish Knowledge AI

## Deploying to Vercel (step by step)

### 1. Push to GitHub
- Create a new repo on github.com
- Upload all these files keeping the same folder structure:
  - api/chat.js
  - public/index.html
  - vercel.json

### 2. Connect to Vercel
- Go to vercel.com and click "Add New Project"
- Import your GitHub repo
- Click Deploy (don't change any settings)

### 3. Add your OpenAI API key
- In your Vercel project, go to Settings > Environment Variables
- Add a new variable:
  - Name:  OPENAI_API_KEY
  - Value: your key (sk-proj-...)
- Click Save

### 4. Redeploy
- Go to Deployments tab and click "Redeploy" on the latest deployment
- That's it! Your site is live and the API key is hidden from users.

### Your folder structure should look like this:
```
hacham/
  api/
    chat.js
  public/
    index.html
  vercel.json
```
