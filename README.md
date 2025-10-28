# Quickqueue
QuickQueue is a smart digital token system with unique features like AI-lite wait time prediction, silent mode alerts, QR code validation, and gamified waiting. It ensures fairness, saves time, and makes queues more engaging, transparent, and eco-friendly for users and businesses.
# QuickQueue — Prototype

A frontend-only prototype for a smart queue management system with Smart ETA, silent notifications, QR-based tokens, coin-based priority skipping, and a mini-game.

Data is stored in your browser’s localStorage and resets when cleared.  
No backend or server setup is required.

---

## Live Prototype

Try the running version here:  
[Open QuickQueue Prototype](https://example.com/quickqueue-prototype)

(Replace the above link with your hosted version or GitHub Pages link once deployed.)

---

## Features

- Service Token Management (create, track, and store tokens locally)
- Smart ETA calculation based on average service time
- Silent Mode using browser vibration API
- Priority control (Normal, VIP, Emergency)
- Voice announcements using SpeechSynthesis API
- Unique QR generation for each token
- Coin-based skip system using a simple quiz mini-game
- Admin & Staff controls (Serve Next, Call Current, Reset Queue)
- Fairness log of last 20 actions
- Export and clipboard copy for queue data

---

## File Structure
quickqueue/
│
├── index.html          # Main file containing HTML, CSS, and JavaScript
├── README.md           # Documentation
---

## How to Use

1. Open index.html in any modern browser.  
   (No installation or server required.)
2. Create a new token with service name, group size, and priority.
3. Use Admin buttons to serve, reset, or manage the queue.
4. Play the quiz to earn coins and spend them to skip spots.
5. View and export current queue details anytime.

---

## LocalStorage Keys

- quickqueue_tokens — Array of all token objects  
- quickqueue_current — Currently serving token number  
- quickqueue_fairness — Fairness log array  
- quickqueue_my_token — User’s own token ID  
- quickqueue_coins — User’s earned coins  
- quickqueue_notify — Notification flag

---

## Technologies Used

- HTML5, CSS3, Vanilla JavaScript  
- Browser APIs: localStorage, SpeechSynthesis, Vibration, Clipboard  
- QR code generation via qrcode.js CDN

---

## Notes

- Works in one browser instance only.  
- Data persists until the browser’s cache is cleared.  
- Use a backend (Firebase or Node.js) for real-time or multi-user capability.

---

## Future Enhancements

- Add Firebase for synchronization across devices  
- Real-time updates using WebSocket  
- Enhanced voice and visual notifications  
- Queue analytics and reports

---
