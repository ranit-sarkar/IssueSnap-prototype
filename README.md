# IssueSnap

**Snap it. Track it. See it fixed.**

IssueSnap is a concept for reporting civic problems (potholes, garbage, broken streetlights and more) with a photo and location, tracking each report step by step, and confirming when it is fixed. It includes an in-app assistant that tells citizens which office handles a problem, what to do next, and where their report stands.

Built by first-year BTech CSE students for Lean In Hacks, the Nexconn Build Challenge 2026 and the West Bengal Seva First Innovation Challenge.

## Live demo

 https://ranit-sarkar.github.io/IssueSnap-prototype/

Tip: open it in one browser tab only (see "Known limits").

## What the prototype shows

- Sign up and log in with a simulated OTP
- Report a problem: category, camera photo, GPS location, note
- Five-step tracker: Received, Sent to authority, Assigned, In progress, Resolved
- Office view to move a report forward, or decline a fake one
- Confirm the fix and earn reward points (a concept)
- English, Hindi and Bengali
- **IssueSnap Assistant** (new in v2):
  - Answers in English, Hindi or Bengali
  - Tells which office handles a problem across India: National Highway (NHAI), state highway (PWD), city or town (municipal body), village (Gram Panchayat, BDO)
  - Looks up the municipal body for major cities
  - Explains how to escalate if nothing happens
  - Shows a 3-step picture of how a typical repair is done (illustrations, not photos)
  - Sends an in-app notification when the office changes the report status

## How the assistant uses Nexconn Chat

- The app uses the Nexconn Chat SDK (web). The citizen connects as one chat user and the assistant as another.
- Every message, and every status update from the office view, travels through Nexconn Chat as a message between the two users.
- The assistant is rule-based. It does not use an AI model and does not call any other service.
- Tokens come from Nexconn for two fixed demo users. The App Secret is never in this repository.

## Known limits

- This is a concept prototype. The OTP, office and report data are simulated. Nothing is sent to any real authority.
- Report data stays in your browser. Only chat messages go through Nexconn.
- Both users are shared demo accounts, so only one active session works at a time.
- The assistant answers from public information and our field research, not live data. Office contacts and helplines should be verified before real use.
- Hindi and Bengali text is machine-assisted and still needs a native-speaker review.

## Version history

- **v1.0**: Prototype without assistant
- **v2.0**: Nexconn Chat assistant, notifications, repair pictures, India-wide guidance

## Credits

Logo concept created with an AI image tool and chosen by our team.
