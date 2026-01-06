# FAST — Instant Dating (India)  
*A consolidated spec + Behance case-study content + AI builder instructions from this chat.*

---

## 0) What FAST is (idea in one breath)
FAST is a dating app designed for **India’s “instant” culture** (quick commerce, reels, low attention spans). Instead of endless chatting, it makes **intent + availability + activity + expectations** visible upfront, so people can move from match → meeting with minimal friction—especially helpful for **busy professionals** and **introverts**.

**Core promise:** *Less talking, more meeting (without the awkwardness).*

---

## 1) Brand & Visual Direction (final palette)
### Primary colors (apply across the entire app)
- **Black (Base):** `#0F1008`  
- **Neon Accent:** `#BEEE02`  

### Supporting neutrals (recommended)
- **Text on dark:** `#F5F7EB`  
- **Muted text:** `#A7AD93`  
- **Surface/Card:** `#17180F`  
- **Divider:** `rgba(190, 238, 2, 0.12)`  

### Neon usage rules
- Neon is **only** for: primary CTAs, active states, key highlights, focus rings, progress/selection indicators.  
- Keep most UI calm/dark; neon is the “spark,” not the wallpaper.

### Color psychology (short, Behance-friendly)
- **Black** signals *premium, confident, modern, distraction-free focus*.  
- **Neon** signals *speed, energy, “instant action,” high clarity*—perfect for FAST’s “quick decision” concept.  
- High contrast also improves scannability and supports rapid decisions.

---

## 2) Brand Identity (logo + glow rules)
### Logo direction
- Use a **logo mark + FAST wordmark**, not plain text-only.
- Style: modern, minimal, geometric (speed / lightning / forward motion cues).
- Neon treatment: soft glow, not harsh.

### Glow rules
- **Glow color:** `#BEEE02`
- **Outer glow:** 12–20px blur, 20–35% opacity
- **Inner glow (optional):** 6–10px blur, 12–18% opacity
- Never glow on large backgrounds—only on the logo or key active elements.

---

## 3) UI/UX Layout Rules (spacing + sizing standards)
Use an **8pt grid** throughout.

### Screen padding & safe areas
- Default screen padding: **16px** left/right
- Section spacing: **24px** between major blocks
- Component spacing: **12–16px** between related elements
- Safe top padding for headers: **16–24px** (depending on device)

### Typography (recommended)
- Display/H1: **28–32px**, Semibold
- H2: **20–22px**, Semibold
- Body: **15–16px**, Regular
- Caption/meta: **12–13px**, Medium
- Line height: **130–150%** depending on size

### Buttons
- Primary button height: **48–52px**
- Corner radius: **14–18px** (modern rounded)
- Horizontal padding: **16–20px**
- Disabled: reduce opacity to **40–50%**

### Cards
- Radius: **18–24px**
- Padding inside card: **16–20px**
- Shadow: minimal (dark UI); rely on elevation via surface color

### Inputs
- Height: **48–52px**
- Radius: **14–16px**
- Focus ring: 2px neon outline (`#BEEE02`) with subtle glow

### Dividers
- 1px height
- Use low-opacity neon-tinted divider or neutral divider
- Divider spacing: **16–20px** vertical

### Icons
- Standard icon size: **20–24px**
- Touch targets: **44px minimum** (even if icon is smaller)

---

## 5) App Flow (current intended UX)
### A) Welcome / Login
**Add login alongside signup**
- Phone number input → “Send OTP”
- OTP screen uses **fake OTP** behavior: auto-fill a dummy OTP to proceed.

### B) Create Profile (Onboarding)
**1) Name + Age**
- Age control must be modern (not old-school steppers).  
  Prefer: slider, segmented control, or clean picker sheet.

**2) Photos**
- “Add Photos” opens a **separate page**.
- User adds **4 photos** then returns to profile.

**3) Bio Builder (no manual typing)**
- “Create Bio” opens a **separate page** with ~10 fast questions.
- Each question has quick selectable options.
- The app auto-generates a short intro/bio from selected answers.

**Bio question examples (fast + personality-revealing)**
- Cat person / Dog person / Both / Neither  
- Coffee / Matcha / Chai / Cold brew  
- Weekend vibe: Home reset / Outdoors / Cafe hopping / Party  
- Movie type: Comedy / Romance / Thriller / True crime  
- Work style: Home / Office / Cafe / Hybrid  
- Fitness: Gym / Run / Yoga / Sports / None  
- Social battery: Extrovert / Ambivert / Introvert  
- Ideal date: Coffee / Drinks / Dinner / Walk  
- Music mood: Indie / Bollywood / Techno / Lo-fi  
- Communication style: Direct / Playful / Soft / Minimal

**4) Bill Preference (currency icon)**
- Replace “bill preference” icon with **₹ (rupee)** icon.
- Options: **Split 50–50 / Alternate / My treat**

### C) Pre-meeting preferences
- Add options: **5-minute voice call** and **5-minute video call**

### D) Activities selection
- Include: Coffee, Movie, Drinks, Dinner, Comedy show, Walk, Museum, Live music, Board games, Dessert, Mental health talk, Books/cafe, Fitness date.

### E) Area selection (move earlier in flow)
- Area selection happens **before** final onboarding completion.
- User types area; open a **bottom sheet** showing:
  - typed area + distance from current location (e.g., “Indiranagar — 2 km”)
  - 3 nearby suggestions (e.g., Indiranagar, Koramangala, HSR)
- Remove “Preferred area” concept.
- Use Bangalore examples only.

### F) Onboarding completion screen
- Full screen success message:  
  “We wish you the best for your date today. Let the search begin.”
- Add a modern illustration/animation matching FAST’s neon-dark theme.

---

## 6) Discovery / Matching (profiles + interactions)
### Profiles (data generation instruction)
- Generate **100+ fake profiles** for swiping/matching.
- Each profile must vary: availability times, interests, activity preferences, personality answers.
- Each profile includes **4 photos**.
- Tinder-like photo viewing: tap to move to next photo.

### Interaction model (latest)
**Replace broken swipe with buttons**
- Show **Like** and **Unlike** buttons (thumbs/tick/cross style).
- Unlike animation: card flies **left** (trash-like motion).
- Like animation: card flies **right** with a **golden glow** accent.
- After a like, show popup: “Send your intro to {Name}” for **5 seconds**.
- Do **not** navigate to chat after swipe/like.
- Show a “Match” popup for **1 out of every 3** likes.

---

## 7) Matches Screen (corrections)
- Show availability as a **time range**, not a single time.
  - Correct format: “6–8 PM”, “7–9 PM”
- Display **name + availability slot** prominently (key decision factor).

---

## 8) Chat Screen (corrections + required behaviors)
### Header content
- Show: **Name, Age**, and **Availability slot**
- Tapping profile photo opens that person’s profile.

### “Send Introduction” behavior
- “Send introduction” must send the **auto-generated intro** built from the Bio Builder answers.
- Place “Send introduction” as a **chat quick-action chip** mixed with other tappable quick messages.


### Keyboard
- Show an on-screen keyboard state in chat UI for realism.

### Add call options
- Add voice call + video call options in chat window.

---

## 9) Time & calendar corrections
- Remove “now” from time slots.
- Add calendar selection so user can pick availability for the **next 7 days**.


---

## 11) Problems & Solutions (your final chosen set)
### Problems (headlines)
- Forced small talk  
- Planning fatigue  
- Mental exhaustion  
- Ghosting cycles  
- Scheduling friction  
- Intent confusion  
- Wastage of time  

### Solutions (headlines)
- Intent-first  
- Clear expectations  
- Auto introductions (no typing)  
- Small talk made easy  
- Time-based matching  
- Availability-led discovery  
- Introvert-friendly flow  
- Quick alignment  

**Rename fix:** Replace “auto introductions and prompts” → **Auto introductions & quick replies**


---

## 13) Key UX definitions
### Journey mapping (meaning)
A journey map is a visual breakdown of the user’s end-to-end experience (steps, thoughts, emotions, pain points, and opportunities) while trying to achieve a goal (here: getting a date quickly without friction).

---

## 14) User Personas (3)
### Persona headings (2–3 words)
1) **Emotional Gen-Z**  
2) **Busy Professional**  
3) **Quiet Introvert**

### Persona 1 — Emotional Gen-Z (Male, 22)
- **Education:** Undergraduate  
- **Lifestyle:** Reels-heavy, fast decisions, social but selective  
- **Needs:** Emotional clarity, vibe match, low effort  
- **Motivation:** Meet someone who “gets it” quickly  
- **Traits:** Expressive, intuitive, impatient with boring chats  
- **Pain point (frustration sentence):**  
  “I’m tired of texting for days just to realize we’re not even on the same vibe.”

### Persona 2 — Busy Professional (Male, 28)
- **Education:** Graduate / Professional diploma  
- **Lifestyle:** Gym, work, routines, high standards, time-poor  
- **Needs:** Efficient filtering, quick planning, confidence in intent  
- **Motivation:** Dating without losing momentum or time  
- **Traits:** Structured, decisive, quality-seeking  
- **Pain point (frustration sentence):**  
  “I don’t have energy for endless back-and-forth that never turns into a real plan.”

### Persona 3 — Quiet Introvert (Male, 30)
- **Education:** Graduate  
- **Lifestyle:** Small circle, thoughtful, prefers calm settings  
- **Needs:** Low-pressure interactions, structured icebreakers, safety  
- **Motivation:** Meet someone without social overload  
- **Traits:** Observant, sincere, anxious about first moves  
- **Pain point (frustration sentence):**  
  “I freeze when chats turn performative—dating apps feel louder than real life.”

### Single Job To Be Done (common goal)
**“Help me quickly find a compatible match and set up a low-effort meeting time without awkward planning or endless chatting.”**

---
