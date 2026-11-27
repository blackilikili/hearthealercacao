# Claude in Chrome prompt: Prosperous Heart Kartra build

Copy everything below the line into Claude in Chrome, with Kartra open and logged in.

---

You are helping Helen Millar set up the email automation for her course **Prosperous Heart** in Kartra. You are working in her live Kartra account, so follow the safety rules exactly.

## Safety rules (these override everything else)

1. **Never delete, archive, rename or overwrite anything that already exists** in Kartra: tags, sequences, automations, pages, products, memberships, lists or contacts. If something existing looks wrong or duplicated, note it in your report and leave it alone.
2. **Never touch the NATM course** or anything belonging to another product. This build is Prosperous Heart only.
3. **Build everything switched off.** Sequences, automations and rules must be saved as inactive or paused. Do not activate anything, and do not subscribe any real contact to anything.
4. **Never send an email** to anyone except a test send to Helen's own address, and only after she has said yes.
5. **Never make a purchase**, test or real, without asking Helen first. A test purchase may charge a card or affect reporting.
6. **Stop and ask** whenever a step would be permanent, or you are unsure which item is the right one, or Kartra's interface does not match these instructions. Explain to Helen what the change would be and that it would be permanent.
7. Use UK English spelling in everything you write, and do not use em dashes.
8. Always spell her name **Helen Millar**.

## Phase 1: Look around first (read only, change nothing)

Find and report back on each of these. Do not build anything in this phase.

1. **The product and membership.** Find the Prosperous Heart product and its membership site. Note the exact product name, membership name, access levels, and how the four chambers are set up (as posts, categories or levels).
2. **Existing tags.** List every tag that already exists, so we reuse rather than duplicate. Note any that look like Prosperous Heart tags already.
3. **Existing sequences and emails.** Look for any Prosperous Heart sequence already in place, especially:
   - **Email 1** (Day 0 welcome). What does it say, and what does it ask people to do on Day 0?
   - **Email 5**. Does it exist? Is it the Flying / Steady / Stuck check-in?
   - Any check-in landing pages for Flying, Steady and Stuck.
4. **Lesson completion triggers.** Open Automations (rules) and check the available triggers. Can Kartra fire a rule when a member **completes** a post or lesson in this membership (not just visits it)? Note the exact trigger names available.
5. **Sequence branching.** Check whether the sequence builder has a condition step (for example "if lead has tag"). Note how it works.
6. **Access terms.** Check the product, membership and sales page for what access buyers get. Is it lifetime access? Quote the wording you find.
7. **The 20 minute call bonus.** Check the Prosperous Heart sales page and product description. Is a 20 minute call with Helen still offered? Is there a booking link or calendar already set up? Quote what you find.
8. **Chamber 2 exercise.** Open the Chamber 2 lesson and its workbook PDF if you can. Email 3 asks people to "tell me which one is the dread". Find the exercise this refers to and summarise it in one or two lines.
9. **Chamber 4 conversation.** Open Chamber 4. Email 6 is titled "One conversation this week" and asks "Reply and tell me how it went". Find the homework or action in Chamber 4 that this refers to (for example, a sales conversation where they say their price out loud).
10. **Merge fields and custom fields.** Find the exact merge tag for first name, and check whether a custom field exists that could hold "last chamber reached".
11. **Sending address.** Note which sender name and address Prosperous Heart emails go from, and whether replies come back to Helen.

Then **stop and send Helen a report**: what you found for each of the 11 points, any problems, and your proposed approach for anything Kartra cannot do as described below. Wait for her to say "go" before Phase 2.

## Phase 2: Build (only after Helen says go)

Build in this order. After each numbered step, tell Helen briefly what you created.

### Step 1. Tags

Create these, reusing any exact or near match you found in Phase 1 (tell Helen which you reused):

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

(The "PH" prefix keeps them separate from NATM. If Helen's existing tags use another convention, ask before choosing.)

### Step 2. Progress tagging

- If Kartra can trigger on lesson completion: create inactive rules so that starting Chamber 1 applies **PH Started**, and completing each chamber applies **PH Completed Chamber N**.
- If it cannot: draft an "I've done this" button for the end of each chamber that applies the matching tag. **Show Helen before adding anything to the membership pages**, as those are live.
- Completing Chamber 4 (or holding all four Completed tags, if Kartra can check that) applies **PH Finished**.
- If a "last chamber reached" custom field is possible, update it each time a Completed tag is applied. If not, tell Helen and suggest wording for Emails 8 and R2 that works without it.

### Step 3. Main sequence: "Prosperous Heart: Welcome and Chambers"

Triggered by purchase (applies **PH Bought**, then subscribes to this sequence). Saved inactive.

| Step | Timing | Who gets it |
|---|---|---|
| Email 1 (existing, from Phase 1) | Day 0 | Everyone |
| Email 2A | Day 2 | Only if NOT tagged PH Started |
| Email 2B | Day 2 | Only if tagged PH Started |
| Email 3 | Day 7 | Everyone |
| Email 4 | Day 14 | Everyone |
| Email 5 (existing, if found) | As found | As found |
| Email 6 | Day 21 | Everyone |
| Email 8 | Day 45 | Only if NOT tagged PH Finished |

**Email 7** is not in this timeline. It goes in its own sequence triggered by **PH Finished**.

### Step 4. Rescue sequences (each saved inactive, each with a stop rule)

- **R1 "Never started"**: subscribe at purchase; send on Day 4 only if NOT tagged PH Started. Stop rule: when PH Started is applied, remove from R1.
- **R2 "Started then paused"**: each time a PH Completed tag is applied, remove from R2 and resubscribe, so the 10 day clock restarts. Send 10 days later if no new Completed tag. Stop rule: any new Completed tag removes them.
- **R3 "The one question"**: same restart method on any progress tag (Started or Completed), sending after 21 days of no progress. Sends once. Stop rule: any progress tag, or after sending.
- If Kartra cannot do the "restart the clock" method, stop and tell Helen what it can do instead.
- Nobody tagged **PH Finished** should receive R1, R2, R3 or Email 8.

### Step 5. One-click reason buttons

In Email 2A and R1, every reason option is a link. Clicking it applies the matching tag and opens the matching landing page.

| Button text | Tag | Landing page |
|---|---|---|
| Time / I haven't had the time | PH Reason: Time | PH Reason: Time |
| Feels like a lot / It feels like a lot | PH Reason: Overwhelm | PH Reason: Overwhelm |
| Not sure it's for me | PH Reason: Expectation | PH Reason: Expectation |
| Tech trouble / I can't get in | PH Reason: Tech | PH Reason: Tech |
| I'm in, just need a nudge / I'm still in, I just need a nudge | PH Reason: Nudge | PH Reason: Nudge |

Note: Email 2A has five options but R1 only has four (no "Not sure it's for me"). Keep R1 as written and flag it to Helen; do not invent new copy for it.

### Step 6. Landing pages

- Five reason pages, using the matching R1 reply text below as the page content, plus a "Back to the course" button to Chamber 1.
- For **PH Reason: Expectation** there is no copy yet. Make the page with a placeholder heading only and tell Helen it needs her words.
- Three check-in pages (Flying, Steady, Stuck): use whatever you found in Phase 1. If nothing exists, create placeholder pages and tell Helen.
- Save all pages as drafts, unpublished.

### Step 7. Write the emails

Use the copy below exactly, with these rules:

- Replace [first name] with Kartra's first name merge tag.
- Every [Button: ...] links to the right place (the chamber lesson, the workbook PDF, the booking link, or a reply link).
- Items in square brackets starting with CONFIRM: fill in from your Phase 1 findings if you found a clear answer, otherwise leave the bracket in and tell Helen.
- Put the subject in the subject line and the preview in the preheader field.
- Sign off as Helen.

## Phase 3: Report and test

1. Send Helen a full summary of everything you built, everything you reused, and every placeholder still open.
2. Ask her whether she wants a test send of each email to her own address, and whether to run a test purchase (and how: coupon, test mode or her own card).
3. **Do not activate anything.** Helen will activate once she has read every email on her phone.

---

## The email copy

Small corrections already made: "No on" to "No one", "unlooked at" to "unlooked-at", and in R1 "they just chunk it down" to "I just chunk it down". Everything else is Helen's wording.

### Email 2A. Day 2, only if Chamber 1 has NOT been started

Subject: Chamber 1 is waiting
Preview: Ten minutes is enough to begin.

Hi [first name],

It's easy to buy something that matters and then let life crowd it out. Let's not let that happen to this one. No one needs another unlooked-at course, so put the time in your calendar for the 4 x 2hr sessions. Break them up however you need. Just get them in the calendar and then...

Press play while you have a cup of tea. Stop when you need to. The point is to begin.

[Button: Press play] (links to Chamber 1)

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

[CONFIRM: one or two lines describing the Chamber 2 exercise found in Phase 1, so "the dread" makes sense. Show Helen a draft before saving.]

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

### Email 6. Day 21, everyone (Chamber 4: Selling, Strategy and Success)

Subject: One conversation this week
Preview: Say the number out loud.

Hi [first name],

Chamber 4 brings it together: selling, strategy and success without losing yourself on the way. Welcome to your Prosperous Heart!

[CONFIRM: one line asking them to have the conversation from the Chamber 4 homework this week, using what you found in Phase 1. Show Helen a draft before saving.]

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

As part of Prosperous Heart you also have a 20 minute call with me to talk through your plans. [CONFIRM THIS BONUS IS STILL OFFERED: if Phase 1 found no evidence of it, leave this paragraph and the button out and tell Helen.]

[Button: Book your 20 minute call]

Helen

### Email 8. Day 45, ONLY if not finished

Subject: Pick it back up
Preview: One chamber, ten minutes.

Hi [first name],

You were last in [last chamber reached], and everything is still here for you [CONFIRM ACCESS TERMS BEFORE SAYING THIS].

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

**Landing page text for each R1 button:**

- **Time:** No worries, these things happen. Get your calendar open now, mark the time in, highlight it, and make it a non-negotiable. This gets to be fun. It gets to bring more money into the business in ways that light you up.
- **Overwhelm:** Overall, this is 8 hours of your life, and you have lifetime access, but rather than putting it off, start small: do 15 minutes and listen to it your way. Sometimes I like to listen to things all the way through before I take action. Other times, I just chunk it down into little sections. Who knows? Some of what's covered you may already be doing, and then there are the learning-curve tweaks that really take things to the next level.
- **Tech:** If you've not received your login link, check your spam and double-check if you're using the same email you signed up with. Any technical problems, respond to this email. (On the page, change "respond to this email" to a reply link or Helen's support address, and tell her which you used.)
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

Your access stays as it is, lifetime access, so you can return whenever you are ready. [CONFIRM ACCESS TERMS: must match what Phase 1 found.]

Helen
