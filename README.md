# Blingo Voice Call Bot System

Blingo's **Voice Call Bot System** is a FastAPI application designed for efficient cold calling. The AI agent engages customers in product discussions with ultra-low latency (<1 second). Using real-time websockets, pre-trained models, and **Elevenslab's** text-to-voice features, users can select a custom voice and initiate calls seamlessly.

---

### Key Technologies

- **Python 3**  
- **FastAPI**  
- **SQLModel ORM**  
- **OpenAI** (response generation)  
- **AWS Transcribe** (speech-to-text)  
- **Twilio** (calling)  
- **Elevenslab** (text-to-voice conversion)  

---

### Features

1. **Secure Authentication**: JWT-based system for user security.  
2. **Real-Time WebSocket Support**: Manage multiple user connections.  
3. **Custom Voice Selection**: Browse and select from available voices.  
4. **Campaign Calls**: Upload customer contact lists (Excel) for sequential calls.

---

### Next Steps

- **Payment Gateway Integration**  
- **Frontend Development**  
- **PostgreSQL Migration**  

---

### Challenges

**Noise in Transcriptions**:  
AWS Transcribe may misinterpret background noise, leading to unexpected AI responses. Implementing noise reduction can resolve this.

---

### Setup

1. Install dependencies:  
   ```bash
   pip install -r requirements.txt
   ```
2. Create a SQLite database file in the project root.  
3. Rename `example.env` to `.env` and add configuration keys.  
4. Launch the server:  
   ```bash
   uvicorn src.main:app
   ```

---

### Team Blingo

**Members**:  
- Ethan Rodrigues  
- Krish Pinto  
- Allen Peter