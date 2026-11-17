# Northside Family Clinic — Practice Operations Dashboard

[![Live Demo](https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-blue?style=for-the-badge&logo=github)](https://mrchandrayee.github.io/northside-clinic-practice-dashboard/)
[![HTML](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org) [![CSS](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org) [![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](./LICENSE)

A runnable frontend reconstruction of the uploaded **11.2-second** screen recording (720 × 1280, 30 fps).

## Run
1. Extract `northside-clinic-practice-dashboard.zip`.
2. Open `index.html` in Chrome, Edge, Firefox or Safari.
3. No npm install or build process is required.

Optional local server:
```bash
python3 -m http.server 8000
```
Then open `http://localhost:8000`.

## What is visible in the video

The recording shows a light mint/white clinic operations interface for **Northside Family Clinic**, with a dark green icon sidebar, top bar showing `10:40 AM Demo day`, and a green `+ New` action.

### 1. Home / Patient flow
Visible metrics:
- Appointments today: **81** (21 seen)
- In the waiting room: **5** (avg 9 min)
- Unread on WhatsApp: **6** (reply in ~8 min)
- No-shows, last 30 days: **4.2%** (was 13% before reminders)

Patient flow sections:
- Expected (50)
- Waiting room (5)
- In consult (5)
- Seen (21)

Patient cards show names, appointment time, clinician, status and contextual actions such as Check in, Call in and Finish.

### 2. Inbox / WhatsApp
Visible metrics:
- 6 unread
- 6 waiting on us
- 8 min median reply
- 10 open conversations

The inbox includes a searchable conversation list with All / Unread / Mine filters, selected patient chat, quick replies (Parking, Opening hours, What to bring, Running late), and a message composer.

A visible conversation is with **Elena Rossi**:
- Incoming: “Do you have parking at the clinic? First time coming to the new building.”
- Reply: “There's free patient parking behind the building — the entrance is on Harbor St, next to the pharmacy.”

### 3. Schedule
The video shows Day and Week schedule modes, clinician chips for Dr. Rahman, Dr. Okafor, Dr. Lin, Dr. Silva and Nurse Berg, appointment cards and a lunch block.

Day view metrics:
- Appointments today: 73
- Booked capacity: 56%
- Open slots today: 20
- Confirmed for Monday: 10% (10 of 73)

Week view metrics:
- Appointments this week: 421
- Booked capacity: 57%
- Open slots today: 25
- Confirmed for Monday: 14% (10 of 73)

A `Send reminders for Monday` action and `New appointment` button are visible.

### 4. Campaigns
Visible WhatsApp broadcast / template screen:
- Messages sent: 3,778
- Read rate: 43%
- Clicked: 14%
- Replies: 1.4%

Broadcasts shown:
- Annual check-up recall · Q4 (Scheduled)
- Well-child check-ups (Draft)
- Holiday hours (Draft)

The video ends with a confirmation dialog for sending **“Well-child check-ups”** to 150 patients; 25 without WhatsApp consent are skipped.

## Source-code extraction note

This video shows the running clinic application UI and interactions. It does **not** show an HTML/CSS/JavaScript editor or readable original source-code panel. Therefore no original source code can be honestly transcribed from this video. The included source files are a fresh frontend implementation reconstructed from the visible screens, labels, metrics and sample content.

## Implemented interactions
- Navigate Home, Inbox, Schedule, Campaigns and supporting sections.
- Patient flow card actions show local demo feedback.
- Search and filter WhatsApp conversations.
- Switch selected patient conversation.
- Send a message locally in the selected chat.
- Quick-reply buttons populate the composer.
- Switch Schedule between Day and Week.
- Appointment and reminder confirmation dialogs.
- Switch Campaigns between Broadcasts and Templates.
- Send confirmation dialog with consent exclusion message.
- Create template / broadcast demo actions.
- Dark theme toggle.

## Files
- `index.html` — app shell and confirmation dialog.
- `styles.css` — responsive clinic UI, patient cards, inbox, calendar and campaign cards.
- `app.js` — local sample data, navigation, chat interactions, schedule modes and confirmation actions.
- `README.md` — source observations and run instructions.

## Limitations
This is a frontend-only recreation. It does not connect to WhatsApp Business API, a live appointment calendar, patient records, an EHR/EMR, SMS provider, clinician scheduling backend or real reminder service. Messages, appointment actions and campaign sends are local demo interactions and do not contact patients.

## 👨‍💻 Author

**mrchandrayee** · [GitHub](https://github.com/mrchandrayee)

## 📄 License

[MIT License](./LICENSE)
