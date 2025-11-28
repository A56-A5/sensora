#  Sensora.ai

> Making the digital world not just accessible, but emotionally inclusive.

---

##  Problem Statement

Imagine a world where everyone experiences content with full emotion. We're bridging the gap between **access** and **feeling**, making the digital world truly inclusive.

---

###  For Blind Users
Flat narration makes every post feel the same — a joke, a breakup, a celebration — all delivered without emotion or human touch. Current tools lack human tone, leaving blind users disconnected from the *feeling* behind posts.

---

###  For Deaf Users
Subtitles often fail to capture emotion. Without vocal cues, users miss out on excitement, sarcasm, anger, or sadness. Meaning is lost without emotional depth.

---

##  Solution

Most accessibility tools focus only on **access**. We’re reimagining that.

Sensora.ai introduces:

-  **Expressive Voice Narration**  
  AI-generated voice that adds tone, pacing, and emotional depth to content — as if a friend is reading it aloud.

-  **Color-Coded Subtitles**  
  Subtitles that show emotional context via color:
  - 🔴 Red = Anger  
  - 🟡 Yellow = Joy  
  - 🔵 Blue = Calm  
  - 🟣 Purple = Sadness  
  - 🟢 Green = Excitement  

---

## Implementation

###  AI-Powered Emotion Engine
Built with **Gemini 1.5 Flash**, our AI engine analyzes social media content and extracts emotional cues for both narration and subtitle enhancements.

###  Web App & Browser Extension
- An accessible **React + Vite** web app
- A browser extension that overlays emotional narration and subtitle cues on platforms like **Instagram** and **Twitter**
- Real-time content enhancement, seamlessly integrated into users' browsing experience

---

##  Tech Stack

| Layer        | Tools/Frameworks                         |
|--------------|------------------------------------------|
| **Frontend** | Vite, TypeScript, React                  |
| **Backend**  | Flask, Python, JavaScript                |
| **AI/ML**    | Google Gemini 1.5 Flash (Generative AI)  |

---

##  Track
**Social and Digital Media**

---

##  Team Members

- **Minhaj Noushad** — AI Developer  
- **Alvi A V** — AI Developer  
- **Merin Binoj** — Frontend Developer  
- **Tharun Krishna C U** — Frontend Developer  

---

##  Vision
We're not just enabling access — we're enabling **emotion**. With Sensora.ai, everyone can feel the digital world, not just see or hear it.

---

# Backend (common for webapp & extnsion)
## Instructions to run 

```bash
git clone https://github.com/A56-A5/sensora
cd backend
```

### Install Dependencies

```bash
pip install Flask flask-cors Pillow requests google-gerativeai
```

Replace this with your gemini api key (50 uses per day (free tier)) in api.py 

```bash
API_KEY = ""
``` 

### Run backend
```bash
python api.py
```

# Web App

## Instructions to run 

Make sure to run the backend in a split / seperate terminal 
```bash
cd web_app
npm install 
npm run dev 
```

Scrolling to each post will out a voice like 
```bash
user John_wick has posted 
Caption : blah blah blah 
Image description : .... 
``` 

Adding new post will call gemini 1.5 flash model to get a detailed image description 
Would load faster than extensions because the api is only called during posting.

# Chrome Extension 

Make sure to run the backend in a split / seperate terminal 
### Installation guide 

1. Go to chrome extensions or copy this link in the browser url 

```bash 
chrome://extensions 
```

2. Enable Developer mode(top right)

3. Click Load unpacked

4. Select Chrome_Extension folder 

5. Your extension should now appear in the Chrome toolbar 

Any changes you make to the code will require a manual Reload of the extension in the extensions page.

Go to twitter home page and click on the extension and it should run 

(Scrolling to new post should update the voice output)

Voice output will be like 
```bash
user John_wick has posted 
Caption : blah blah blah 
Image description : .... 
``` 


## Screenshots

![App Screenshot](images/image.png)
![App Screenshot](images/image2.png)
