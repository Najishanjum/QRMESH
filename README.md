<div align="center">
<img width="1200" height="475" alt="GHBanner" src="https://ai.google.dev/static/site-assets/images/share-ais-513315318.png" />
</div>

📱 What is QRMesh?
QRMesh is an app that lets you send images or audio between two devices using only QR codes — no internet or servers needed. It works purely through light (your screen displays QR codes, another device's camera scans them).

🚀 How to Use It
You need two devices (e.g., your laptop + your phone, or two phones):

Device 1 — The Sender (Transmit mode)
Open http://localhost:3000/ on the sending device
Click "Transmit" tab (selected by default)
Click the upload area and select a photo or short audio file (audio must be < 5MB)
Wait for the file to be compressed and split into chunks
Hit "Play" — the app will start cycling through QR codes rapidly on screen
Adjust the Speed slider if needed (slower = more reliable scanning)
Device 2 — The Receiver (Scan mode)
Open http://localhost:3000/ on the receiving device (or use http://10.38.82.236:3000/ from your phone on the same WiFi)
Click "Scan" tab
Click "Start Scanner" and allow camera access
Point the camera at the sender's screen showing the cycling QR codes
Watch the LEGO-style blocks fill in as chunks are captured
Once all chunks are received, the image/audio is automatically reassembled and displayed! 🎉
📤 How to Share / Send This App to Others
You have a few options:

Method	How
Same WiFi network	Others on your WiFi can open http://10.38.82.236:3000/ right now while your dev server is running
Share the project folder	Zip the qrmesh (1) folder and send it via Telegram/WhatsApp/email. They just need to run npm install then npm run dev
Deploy online	Deploy to Vercel, Netlify, or Firebase Hosting so anyone can access it from a URL
Would you like me to deploy this online (e.g., to Vercel or Netlify) so you get a public shareable link?
# Run and deploy your AI Studio app

This contains everything you need to run your app locally.

View your app in AI Studio: https://ai.studio/apps/d5e62cb4-45e9-4c94-a234-1fb45255b1d4

## Run Locally

**Prerequisites:**  Node.js


1. Install dependencies:
   `npm install`
2. Set the `GEMINI_API_KEY` in [.env.local](.env.local) to your Gemini API key
3. Run the app:
   `npm run dev`
