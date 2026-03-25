# Dat'n — AI Dating App

_Last updated: 2026-03-24_

**Domain:** datn.ai  
**Legal entity:** Matter Media LLC (DBA TBD)  
**Status:** Concept / Pre-build  
**Platform:** Mobile app (iOS + Android) — consumer product

---

## The Concept

Dat'n is an AI-powered dating app that actually gets you dates. Less swiping, more results. Powered by an AI wingman named **Dante** who guides you through every step — profile, openers, conversations, date planning.

**Positioning:** The anti-Tinder. No endless swiping into the void. Dante does the work.

---

## The Brand

- **App name:** DAT'N (blocky letters, bold/stencil style)
- **AI mascot:** Dante
- **Domain:** datn.ai
- **Tone:** Confident, direct, a little witty. Not soft, not cheesy.
- **Vibe:** Streetwear meets tech. Bold. Like Supreme if it made a dating app.

### Name Logic
- DAT'N = contraction of "dating" — instantly understood
- Dante is hidden inside the brand name
- Dante the poet spent his life chasing love (Beatrice) — subtle literary depth
- In the Inferno, Dante guides people through hell — your Dante guides people through the hell of modern dating

### Tagline Options
- *"Let Dante do the work"*
- *"Your guide through modern dating"*
- *"Dat'n. Powered by Dante."*
- *"Stop swiping. Start dating."*

---

## Dante — The AI

Dante is your personal dating concierge. He's seen everything, judges nothing, and exists solely to get you dates.

### What Dante Does
- **Profile optimization** — rewrites your bio, selects best photos, maximizes match rate
- **Opener generation** — crafts personalized openers based on the other person's profile
- **Conversation coaching** — suggests replies in real-time, keeps things moving
- **Date planning** — recommends venues, timing, how to ask
- **Post-date debrief** — what went well, what to do next, when to follow up

### Dante's Personality
- Smooth, knowledgeable wingman
- Brutally honest when needed (your profile needs work — here's why)
- Warm but not a pushover
- Never robotic, always human-feeling

---

## Core Features (MVP)

1. Profile builder with Dante feedback
2. AI-generated openers (paste their profile, get 3 options)
3. Conversation assistant (screenshot chat, get reply suggestions)
4. Match scoring — Dante rates compatibility and explains why
5. Date idea generator based on location + vibe

---

## Build Strategy

**Mobile-first. Consumer product.**

### Phase 1 — Web App (Months 1-2)
- Mobile-responsive web app at datn.ai
- Faster to build, no App Store delays
- Validate Dante's features with real users
- Build waitlist + early adopter base

### Phase 2 — Native App (Months 3-6)
- React Native or Flutter (one codebase → iOS + Android)
- Submit to App Store + Google Play
- This is when marketing kicks into high gear

### Phase 3 — Scale
- Push notifications, location features, deeper integrations
- Tinder/Hinge/Bumble companion features

---

## Roadmap

### 🟢 Easy (This week)
- [x] Register datn.ai domain ✅
- [ ] Set up Cloudflare DNS + email forwarding (hello@datn.ai, dante@datn.ai)
- [ ] Register DBA under Matter Media LLC
- [ ] Create OpenRouter account for LLM routing
- [ ] Set up GitHub repo
- [ ] Define Dante's personality/voice doc

### 🟡 Medium (This month)
- [ ] Brand design — logo, color palette, font system
- [ ] Landing page with waitlist capture at datn.ai
- [ ] Dante MVP — profile review tool (mobile web form, Dante responds)
- [ ] Set up Stripe for payments (web checkout to avoid 30% App Store cut)
- [ ] Define pricing model
- [ ] Set up Supabase for auth + user data

### 🔴 Hard (Months 1-3)
- [ ] Full mobile-responsive web app
- [ ] User accounts + profile storage
- [ ] Conversation coaching feature (screenshot → Dante suggests reply)
- [ ] Real-time chat interface with Dante
- [ ] OpenRouter multi-model routing (fast model for quick replies, smart model for strategy)

### 🔵 Native App (Months 3-6)
- [ ] React Native or Flutter app
- [ ] iOS App Store submission
- [ ] Google Play submission
- [ ] Push notifications
- [ ] Location-based date suggestions
- [ ] Dante voice mode (talk to your wingman via ElevenLabs)

### 🚀 Later (Scale)
- [ ] Tinder/Hinge/Bumble integration layer
- [ ] Social features
- [ ] Partnership with dating apps
- [ ] Referral program
- [ ] Premium tiers + credits system

---

## Monetization

**Strategy:** Web-based subscription to avoid 30% App Store cut. App is free to download, upsells to datn.ai checkout.

- **Free tier** — limited Dante interactions (3 openers/day, 1 profile review)
- **Dat'n Pro — $19/mo** — unlimited openers, conversation coaching, date planning
- **Dat'n Elite — $29/mo** — everything + priority Dante, voice mode, advanced profile analytics
- **One-time packages** — "Profile Makeover" $49, "First Week Coaching" $29

---

## Tech Stack
- **LLM routing:** OpenRouter (model-agnostic, fallbacks built in)
- **Auth + DB:** Supabase
- **Payments:** Stripe (web checkout)
- **Mobile:** React Native or Flutter (Phase 2)
- **Email:** Cloudflare routing → Gmail (upgrade to Google Workspace later)
- **Hosting:** Vercel (web app)

---

## Notes
- datn.ai registered 2026-03-24 (GoDaddy, 2yr + protection)
- daten.ai was unavailable — datn.ai is the play
- Consumer mobile app — dating is phone-first behavior
- Bypass App Store 30% cut with web subscription model
- Same core stack as Hired AI — build once, reuse across both projects
