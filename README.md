# Neural Conjecture Proposer — Vercel Edition

## 🚀 Deploy (Drag-and-Drop)

1. Extract this ZIP
2. Go to [vercel.com](https://vercel.com) → Sign up with GitHub
3. Click **Add New Project** → **Upload** → drag the extracted folder
4. Framework should show **"Other"** (correct)
5. Click **Deploy**
6. After deploy, click **Go to Dashboard**
7. Click **Settings** → **Environment Variables**
8. Add: `GROQ_API_KEY` = ``
9. Go to **Deployments** → three dots → **Redeploy**

## ✅ Verify

Visit `https://YOUR-URL.vercel.app/api/health`

Should return: `{"status":"ok","keyConfigured":true}`

## 📝 Notes

- Batch capped at 5 conjectures to stay inside Vercel's 10s free timeout
- All API calls are concurrent (not sequential) to beat the timeout
- If batch still times out, reduce to 2–3 in the UI
