# Pose Classification 🧍 · Moonlight ML Workshop

A web app that **recognises your body pose through the webcam** and turns it into sound, using a custom pose model trained with Google Teachable Machine.

Built while learning during the **Moonlight Machine Learning Workshop** (trainer: Naveen).

## 🎬 Demo
Watch **`Pose Project.mp4`** in this repo to see it running live.

## ✨ How it works
Each webcam frame goes through PoseNet to find body keypoints, then the Teachable Machine pose model predicts which pose you are making. The confidence controls a tone: the surer the model is, the higher and louder the sound.

## 🛠️ Tech Stack
[Google Teachable Machine](https://teachablemachine.withgoogle.com/) (model training) · [Teachable Machine Pose library](https://github.com/googlecreativelab/teachablemachine-community) + TensorFlow.js · [p5.js](https://p5js.org/) (canvas, webcam, sound) · JavaScript

## 🚀 Run it
1. Download or clone this repo
2. Serve the folder with any local server (browsers block webcam/mic on plain files), for example:
   ```bash
   python -m http.server 8000
   ```
3. Open **http://localhost:8000** and allow camera/microphone access
4. Click once on the page to enable sound

Or publish it free with **GitHub Pages**: *Settings → Pages → Deploy from branch → `main`*.

## 📚 What I learned
- Training a custom ML model without code using Teachable Machine
- Loading a trained model in the browser and running predictions in real time
- Turning predictions into interactive output (visuals and sound)

## 👤 Author
**Lohith K** · [GitHub](https://github.com/Amulpappu) · [LinkedIn](https://www.linkedin.com/in/lohith-k-b1331a3a8/)
