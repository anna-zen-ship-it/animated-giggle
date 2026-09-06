# Anna & Ren Podcast

🎧 A university podcast hosted by Anna and Ren — fictional student storytellers created as personas to explore inspiring topics from everyday life to timeless ideas.  
Calm, warm, and conversational, each episode invites listeners into a friendly dialogue that blends curiosity with reflection.

---

## ✨ Description
This repository documents the creative journey of **Anna & Ren Podcast**.  
It serves as a hub for scripts, notes, and production details behind each episode — blending narrative, sound design, and thoughtful dialogue.

---

## 👥 Host Personas
- **Anna**  
  A curious and reflective voice, Anna brings warmth and calm energy to each conversation.  
  She represents the mindful side of storytelling — attentive, poetic, and grounded.

- **Ren**  
  A lively and inquisitive student, Ren adds spontaneity and fresh perspectives.  
  He represents curiosity, humor, and the joy of exploring new ideas.

*(Both are fictional personas created to embody different tones of narration and dialogue.)*

---

## 🎙️ Episode Format
- **Opening Reflection** → A short thought or quote to set the mood  
- **Main Dialogue** → Anna & Ren discuss a topic from everyday life or timeless ideas  
- **Ambient Layering** → Background piano or subtle soundscapes for atmosphere  
- **Closing Note** → A gentle takeaway, inviting listeners to reflect further  

---

## 🌱 Vision
The Anna & Ren Podcast is a space for:  
- Exploring everyday stories with depth and curiosity  
- Blending **Zen-style calmness** with **student-like spontaneity**  
- Creating bilingual narration experiments (Thai/English)  
- Inspiring listeners to pause, reflect, and grow together  

---

## 📂 Repository Structure
- `scripts/` → Episode drafts & dialogue  
- `notes/` → Creative notes, reflections, and checklists  
- `audio/` → Sound design references & ambient tracks  
- `assets/` → Visuals, cover art, and promotional materials  

---

🌸 Welcome to the Anna & Ren Podcast repo — a creative sandbox where fictional voices bring real inspiration to life.
## 🎧 Demo Mode
🔗 [Try the Demo on Google AI Studio](https://aistudio.google.com/apps/f09d1c85-7f91-4cb4-aa8f-d82c577d8fdb?showAssistant=true&showPreview=true)
---

## ⚠️ Known Limitations

### Gemini 3.1 Flash TTS Quota
- **Quota Limit**: Flash TTS มีข้อจำกัดการใช้งาน (429 Too Many Requests) เมื่อถึงจำนวนครั้งสูงสุดต่อวัน  
- **Fallback Behavior**: เมื่อ quota หมด ระบบจะสลับไปใช้ **Acoustic Narration Fallback** โดยอัตโนมัติ  
- **Reset Cycle**: Quota จะรีเซ็ตทุก 24 ชั่วโมง

### Demo Mode vs. Live API
- **Demo Mode**: ใช้ environment variable (`DEMO_MODE="true"`) หรือ request payload (`forceDemo: true`) เพื่อจำลองผลลัพธ์  
- **Live API**: หากมี `GEMINI_API_KEY` ระบบจะเรียก Gemini 3.1 Flash TTS จริง  
- **Fallback Handling**: หาก API call ล้มเหลว ระบบจะกลับไปใช้ Demo Mode หรือ Acoustic narration

### Vite Dev Server / WebSocket
- **Error**: `[vite] failed to connect to websocket (Error: WebSocket closed without opened.)`  
- **Cause**: เกิดจาก dev server crash, network block, หรือ client เชื่อมต่อก่อน server พร้อม  
- **Impact**: Hot‑reload อาจไม่ทำงาน แต่การ preview หลักยังคงทำงานได้  
- **Workaround**: Restart dev server (`npm run dev`), ตรวจสอบ port (5173), และเพิ่ม error handling สำหรับ WebSocket

---

✨ หมายเหตุ: Repo giggle เป็น **playground** สำหรับการทดลอง narration และ TTS จึงอาจพบ error หรือ fallback ได้เป็นเรื่องปกติ — *เสียงหัวเราะเบา ๆ แม้จะ error* 🌿

🌿 *This project runs in Demo Mode — safe to explore, no real API calls, no costs. *
Animated Giggle — A playful repo for creative experiments, narration drafts, and demo links. 
Hosted by Anna & Ren, blending curiosity with calm reflections. 
Safe Demo Mode included — explore freely without costs.
