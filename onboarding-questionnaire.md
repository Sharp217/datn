# Dat'n — Dante Onboarding Questionnaire

_The questions Dante asks every new user before coaching them._
_Goal: Build a complete dating profile so Dante can give personalized, relevant advice from day 1._

---

## The Experience

Conversational, not a form. Dante asks one question at a time, responds warmly to each answer, then moves to the next. Feels like talking to a friend, not filling out a survey.

Tone: confident, casual, a little witty. Like your cool older friend who's seen everything.

---

## The Questions (in order)

### 1. The Basics
**Dante says:**
> "Alright, before we get into it — tell me a little about yourself. How old are you and where are you based?"

**Captures:** Age, city/location
**Why:** Tailors advice to local dating scene and age-appropriate dynamics

---

### 2. What They're Looking For
**Dante says:**
> "Good. Now — what are you actually looking for right now? Be honest, I don't judge."

**Options (tap to select):**
- Something serious / long-term relationship
- Casual dating, keeping it fun
- Not sure yet — just seeing what's out there
- Getting back out there after a break

**Why:** Fundamentally changes Dante's coaching approach

---

### 3. Current Situation
**Dante says:**
> "Where are you at right now? Are you actively on any apps, or more of an in-person kind of person?"

**Options:**
- Active on dating apps (Tinder, Hinge, Bumble, etc.)
- Mostly meet people in real life
- Both
- Just getting started, not sure yet

**Why:** Determines whether to focus on app strategy vs. real-life skills

---

### 4. Dating Apps (if applicable)
**Dante says:**
> "Which apps are you on? Select all that apply."

**Options:** Tinder / Hinge / Bumble / Coffee Meets Bagel / Match / Raya / Feeld / Grindr / Scruff / Other / None

**Why:** Platform-specific advice (Hinge prompts vs. Tinder openers are different)

---

### 5. Biggest Challenge
**Dante says:**
> "Real talk — what's your biggest struggle right now? Where do you feel like things break down?"

**Options:**
- Getting matches in the first place
- Coming up with what to say (openers)
- Keeping conversations going
- Getting to the date — things fizzle before we meet
- The date itself — I freeze up or it doesn't go well
- After the date — I don't know how to follow up
- All of the above honestly 😅

**Why:** Dante knows where to focus first

---

### 6. Past Experience
**Dante says:**
> "How would you describe your dating experience overall? Not judging, just want to know what we're working with."

**Options:**
- Pretty new to this — limited experience
- Some experience, had a few relationships
- Decent amount of experience, just in a dry spell
- Very experienced, just need a tune-up
- Just got out of something serious

**Why:** Calibrates how basic or advanced Dante's advice should be

---

### 7. What Matters to Them
**Dante says:**
> "Last one — what matters most to you in a potential partner? Pick your top 3."

**Options:**
- Physical attraction
- Emotional connection
- Shared interests / hobbies
- Ambition / drive
- Humor
- Kindness / empathy
- Lifestyle compatibility (fitness, social, travel)
- Intellectual connection
- Values alignment
- Spontaneity / adventure

**Why:** Helps Dante understand what to optimize for in profiles and conversations

---

### 8. Profile Review (optional but recommended)
**Dante says:**
> "Want to start with a profile review? Drop your best photo and I'll tell you exactly what's working and what's not."

**Action:** Upload photo OR skip for now

**Why:** Immediate value — Dante gives a first win right away

---

## After the Questionnaire

**Dante summarizes:**
> "Okay, I've got you. Here's what I'm seeing: [personalized summary based on answers]
> 
> Here's where we're going to start: [specific first recommendation]
>
> Let's get to work. 👊"

---

## Technical Notes

- Store all answers in Supabase under `user_profile` table
- Used to personalize ALL future Dante responses
- Allow user to update answers anytime in settings
- Use answers as system context when calling Anthropic (OpenRouter DELETED Apr 1)
- Re-ask annually or when user indicates major life change ("just got out of a relationship")

---

## Dante's System Prompt (generated from answers)

After questionnaire, dynamically build Dante's context:

```
User profile:
- Age: {age}, Location: {city}
- Looking for: {relationship_goal}
- Current situation: {dating_situation}
- Apps: {apps}
- Biggest challenge: {challenge}
- Experience level: {experience}
- What they value: {values}

Coach this user accordingly. Their biggest focus area right now is {challenge}.
```
