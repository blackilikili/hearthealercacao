# Claude in Chrome prompt: Prosperous Heart Kartra build

Copy everything below the line into Claude in Chrome, with Kartra open and logged in.

---

You are helping Helen Millar set up the email automation for her course **Prosperous Heart** in Kartra. You are working in her live Kartra account, so follow the safety rules exactly.

## Safety rules (these override everything else)

1. **Never delete, archive, rename or edit anything that already exists** in Kartra: tags, sequences, automations, pages, products, memberships, lists or contacts. If something existing looks wrong, note it in your report and leave it alone.
2. **Do not touch the existing post-purchase login email** or its sequence ("The Prosperous Heart Welcome"). It stays exactly as it is.
3. **Never touch the NATM course** or anything belonging to another product.
4. **Build everything switched off.** New sequences and automations must be saved inactive. Do not activate anything, and do not subscribe any real contact to anything.
5. **Never send an email** to anyone, and never make a purchase, test or real, without asking Helen first.
6. **Stop and ask** whenever a step would be permanent, you are unsure which item is the right one, or Kartra does not match these instructions. Explain the change and that it would be permanent.
7. **Use Helen's email copy exactly as written below.** Do not reword, shorten or add to it.
8. Use UK English spelling in anything you write yourself, and no em dashes. Always spell her name **Helen Millar**.

## What is already known

- The chamber videos are hosted in Kartra, so progress is tracked with Kartra's video triggers.
- Access is lifetime access.
- The 20 minute call bonus is still offered. The booking link is hearthealer.co.uk/free-call/
- No existing tags clash with the new "PH" tags below.

## Build order

After each step, tell Helen briefly what you created.

### Step 1. Tags

Create:

- PH Bought
- PH Started
- PH Completed Chamber 1
- PH Completed Chamber 2
- PH Completed Chamber 3
- PH Completed Chamber 4
- PH Finished
- PH Flying
- PH Steady
- PH Stuck
- PH Reason: Time
- PH Reason: Overwhelm
- PH Reason: Expectation
- PH Reason: Tech
- PH Reason: Nudge

### Step 2. Progress tracking (inactive automations)

Using the video triggers ("contact plays video" and "contact completes video", or the nearest names Kartra shows):

- Plays the Chamber 1 video: apply **PH Started**
- Completes the Chamber 1 video: apply **PH Completed Chamber 1**
- Completes the Chamber 2 video: apply **PH Completed Chamber 2**
- Completes the Chamber 3 video: apply **PH Completed Chamber 3**
- Completes the Chamber 4 video: apply **PH Completed Chamber 4** and **PH Finished**
- Purchase of Prosperous Heart: apply **PH Bought**

If a chamber has more than one video, ask Helen which video counts.

### Step 3. Main sequence: "PH Chambers" (new, inactive)

Triggered by purchase of Prosperous Heart. The existing login email already covers Day 0, so this sequence starts at Day 2.

| Email | Timing | Who gets it |
|---|---|---|
| Email 2A | Day 2 | Only if NOT tagged PH Started |
| Email 2B | Day 2 | Only if tagged PH Started |
| Email 3 | Day 7 | Everyone |
| Email 4 | Day 14 | Everyone |
| Email 6 | Day 21 | Everyone |
| Email 8 | Day 45 | Only if NOT tagged PH Finished |

**Email 7** goes in its own new inactive sequence, "PH Finished", triggered by the tag **PH Finished**.

### Step 4. Rescue sequences (new, inactive, each with a stop rule)

- **R1 "PH Never started"**: start at purchase; send on Day 4 only if NOT tagged PH Started. Stop rule: when PH Started is applied, remove them from R1.
- **R2 "PH Paused"**: each time a PH Completed tag is applied, remove from R2 and resubscribe, so the 10 day clock restarts. Sends after 10 days with no new Completed tag. Stop rule: any new Completed tag.
- **R3 "PH One question"**: same restart method on any progress tag (Started or Completed), sending after 21 days of no progress. Sends once. Stop rule: any progress tag, or after sending.
- Nobody tagged **PH Finished** receives R1, R2, R3 or Email 8.
- If Kartra cannot do the "restart the clock" method, stop and tell Helen what it can do instead.

### Step 5. One-click reason links

In Email 2A and R1, every reason option is a Kartra tracking link that applies the tag and opens the matching page.

| Button text | Tag | Page |
|---|---|---|
| Time / I haven't had the time | PH Reason: Time | PH Reason: Time |
| Feels like a lot / It feels like a lot | PH Reason: Overwhelm | PH Reason: Overwhelm |
| Not sure it's for me (Email 2A only) | PH Reason: Expectation | PH Reason: Expectation |
| Tech trouble / I can't get in | PH Reason: Tech | PH Reason: Tech |
| I'm in, just need a nudge / I'm still in, I just need a nudge | PH Reason: Nudge | PH Reason: Nudge |

### Step 6. Pages (save as unpublished drafts)

**Five reason pages.** Use Helen's R1 reply text (below) as the page content, with a "Back to the course" button to Chamber 1. "PH Reason: Expectation" has no text from Helen yet: build it with the heading only and tell her it needs her words.

**Three check-in pages: PH Flying, PH Steady, PH Stuck.** Helen has not written the check-in email or page text yet. Build each page with its heading only ("Flying", "Steady", "Stuck") and a "Back to the course" button. Also create three tracking links that apply PH Flying, PH Steady or PH Stuck and open the matching page, ready for Helen's check-in email later. **Do not write or build the check-in email.**

### Step 7. Write the emails

- Replace [first name] with Kartra's first name merge tag.
- Every [Button: ...] links to the right place: the chamber lesson, the workbook PDF, the booking link, or a reply link.
- [last chamber reached] and [last lesson reached]: if Kartra cannot fill these automatically, tell Helen and wait for her decision. Do not reword the sentence yourself.
- Subject goes in the subject line, preview in the preheader field.

## When you have finished

1. Send Helen a summary of everything you created, and anything still waiting on her (the Expectation page text, the check-in pages and email, and the last-chamber merge field if needed).
2. Tell Helen: the membership access level "Standard" shows 3 posts but there are four chambers. Check that buyers can open Chamber 4. Do not change it yourself.
3. Ask whether she wants test sends to her own address. **Do not activate anything.**

---

## Helen's email copy

Only one change from Helen's original: the typo "No on" is now "No one".

### Email 2A. Day 2, only if Chamber 1 has NOT been started

Subject: Chamber 1 is waiting
Preview: Ten minutes is enough to begin.

Hi [first name],

It's easy to buy something that matters and then let life crowd it out. Let's not let that happen to this one. No one needs another unlooked at course, put the time in your calendar for the 4 x 2hr sessions. Break them up however you need. Just get them in the calendar and then...

Press play while you have a cup of tea. Stop when you need to. The point is to begin.

[Button: Press play]

What's in the way?

[Time] [Feels like a lot] [Not sure it's for me] [Tech trouble] [I'm in, just need a nudge]

Helen

### Email 2B. Day 2, only if Chamber 1 HAS been started

Subject: You've begun. Here's the next move.
Preview: Open the workbook while it's fresh.

Hi [first name],

You've started, which matters more than it sounds. Every journey to greatness starts with the first step.

Open the Chamber 1 PDF and do the homework page while the teaching is fresh. It is the difference between feeling inspired and having something to act on.

[Button: Open the Chamber 1 workbook]

Helen

### Email 3. Day 7, everyone (Chamber 2: Grounded, Sustainable, Growth)

Subject: Growth that doesn't burn you out
Preview: Chamber 2, plus one small exercise.

Hi [first name],

Growth that costs you everything isn't growth you can keep.

Chamber 2 is about building the kind that is grounded, juicy and sustainable.

[Button: Watch Chamber 2]

Hit reply and tell me which one is the dread.

Helen

### Email 4. Day 14, everyone (Chamber 3: Pricing, Integrity and Value)

Subject: The chamber people avoid
Preview: Pricing is where the heart meets the numbers.

Hi [first name],

Chamber 3 is the one people put off, and it is often the one that changes the most.

Pricing. It's where the reward lies; notice if there is an ick, we work through that to epic results.

[Button: Watch Chamber 3]

How much do you want to receive in the next year?

When I started this work, I couldn't believe where I am now. I would have fallen off my chair and probably not got up.

Yes, at the beginning, this felt overwhelming, but now, after multiple companies, properties, and portfolios, expanding my financial knowledge is something I enjoy.
It doesn't have to be complicated.
The juice is most definitely worth the squeeze.

Let's go!

Helen

### Email 6. Day 21, everyone (Chamber 4: Selling, Strategy & Success)

Subject: One conversation this week
Preview: Say the number out loud.

Hi [first name],

Chamber 4 brings it together: selling, strategy and success without losing yourself on the way. Welcome to your Prosperous Heart!

[Button: Watch Chamber 4]

Reply and tell me how it went.

Helen

### Email 7. On completion (triggered by PH Finished)

Subject: You finished. What shifted?
Preview: Three lines from you would mean a lot.

Hi [first name],

You have been through all four chambers. That is a real commitment, to your work and to yourself. Hats off, as we say in the UK.

Would you reply with three lines?

Where were you when you started?
What has changed in how you price or sell?
What would you tell someone about to begin?
With your permission I'd love to share your words, and if you'd rather keep them private, say so.

As part of Prosperous Heart you also have a 20 minute call with me to talk through your plans.

[Button: Book your 20 minute call] (links to hearthealer.co.uk/free-call/)

Helen

### Email 8. Day 45, ONLY if not finished

Subject: Pick it back up
Preview: One chamber, ten minutes.

Hi [first name],

You were last in [last chamber reached], and everything is still here for you.

No catching up needed. Just one chamber and one page of the workbook.

[Button: Resume where I left off]

Helen

### R1. Day 4, never started

Subject: What's in the way?
Preview: Tap the closest one.

Hi [first name],

Something in you said yes to this course, and that yes still counts.

It's been a few days and the first lesson hasn't been opened, which is very common. It is rarely about willpower. It's usually one of these. Tap the closest:

[I haven't had the time]
[It feels like a lot]
[I can't get in]
[I'm still in, I just need a nudge]

Helen

**Reason page text (one page per button):**

- **Time:** No worries, these things happen. Get your calendar open now, mark the time in, highlight it, and make it a non-negotiable. This gets to be fun. It gets to bring more money into the business in ways that light you up.
- **Overwhelm:** Overall, this is 8 hours of your life, and you have lifetime access, but rather than putting it off, start small: do 15 minutes and listen to it your way. Sometimes I like to listen to things all the way through before I take action. Other times, they just chunk it down into little sections. Who knows? Some of what's covered you may already be doing, and then there are the learning-curve tweaks that really take things to the next level.
- **Tech:** If you've not received your login link, check your spam and double-check if you're using the same email you signed up with. Any technical problems, respond to this email.
- **Nudge:** You're welcome.

### R2. Day 10 of no progress, started but stopped

Subject: You paused. That's allowed.
Preview: Money work can stir things up.

Hi [first name],

You began, and then life, or something deeper, asked for your attention.

Work on money and worth can stir things up. Pausing is part of the process. Letting it go quiet forever is a different thing, and I bet the more prosperous version of you wishes you didn't. Whatever you tell yourself about it that is getting in the way of completing, you have to stay with it to see if you are right, or deliciously wrong!

Pick it up with ten minutes at [last lesson reached].

[Button: Resume where I left off]

Or tell me what's true right now by replying to this.

Helen

### R3. Day 21, the one question

Subject: One question before I close the loop
Preview: Your answer shapes how I teach this.

Hi [first name],

One question, and it takes less than a minute: what would have made this easier to finish?

[Button: Tell me in one line] (a reply link to Helen's sending address)

There is no right answer, and nobody is judged. Your reply helps me teach this better for the next person.

Your access stays as it is, lifetime access, so you can return whenever you are ready.

Helen
