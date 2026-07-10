# Day 3 — Role-Based Prompting

## What I learned
Role-based prompting means giving Claude a persona (e.g. "You are a registered dietitian")
before asking a question. This changes the tone, vocabulary, structure, and depth of the
answer — without changing the underlying facts Claude knows. The same question can come
back sounding clinical, blunt, or warm and casual, purely based on the role assigned.

---

## Response A — No Role
**Prompt used:**
```
How should I approach eating healthier?
```
**Claude's response:**
> Good goal to have. Here's a practical way to think about it:
>
> **Start with what you add, not what you cut**
> Rather than banning foods, try adding more vegetables, fruits, whole grains, and protein to your meals. This crowds out less nutritious options naturally and feels a lot less like deprivation.
>
> **Build meals around protein and fiber**
> These two keep you full longest, which makes everything else easier — less snacking, more stable energy. A meal with a protein source (eggs, beans, chicken, fish, tofu, yogurt) plus fiber (vegetables, fruit, whole grains) is a solid template to reach for.
>
> **Cook more of your own food when you can**
> Not because restaurant or packaged food is "bad," but because cooking gives you control over ingredients and portions without having to think hard about it.
>
> **Don't aim for perfect**
> The people who eat well long-term aren't the ones with the strictest rules — they're the ones with sustainable habits. An 80/20 approach (mostly nutritious, some room for whatever you enjoy) beats a rigid plan you abandon in three weeks.
>
> **Small, specific changes over sweeping overhauls**
> Instead of "eat healthy," try something concrete: "add a vegetable to dinner," "swap soda for sparkling water three days a week," "eat breakfast with protein in it." Specific and small tends to stick.
>
> **Watch out for these common traps**
> - Skipping meals and then overeating later
> - Treating "healthy" as all-or-nothing (one imperfect meal doesn't ruin anything)
> - Copying someone else's diet without considering your own life, budget, or preferences
>
> If you want, tell me a bit about your current eating habits, schedule, or what you're hoping to change (more energy, weight goals, just feeling better) and I can help you build something more tailored.

**Usage after this response:**
![Usage after Response A](screenshots/usage-a.png)

---

## Response B — Dietitian Role
**Prompt used:**
```
You are a registered dietitian with 15 years of clinical experience. How should I approach eating healthier?
```
**Claude's response:**
> Great goal — and the good news is you don't need a complicated plan to make real progress. Here's how I'd approach it with a client starting out:
>
> **1. Start with addition, not restriction**
> Instead of focusing on what to cut out, focus on what to add: more vegetables, more protein, more fiber, more water. This naturally crowds out less nutritious choices without the mental burden of "forbidden foods," which tends to backfire long-term.
>
> **2. Build meals around a simple template**
> A useful mental model for most meals:
> - A palm-sized portion of protein (eggs, fish, chicken, beans, tofu, Greek yogurt)
> - A fist-sized portion of vegetables or more
> - A cupped-hand portion of whole grains or starchy carbs (rice, oats, potatoes, whole wheat)
> - A thumb-sized portion of healthy fats (olive oil, nuts, avocado)
>
> This isn't about precision — it's a rough guide that gets you balanced meals without counting anything.
>
> **3. Prioritize consistency over perfection**
> Sustainable eating habits beat "perfect" diets that collapse in three weeks. Aim for what you can realistically keep doing — 80% of meals aligned with your goals is far more valuable than 100% for two weeks then giving up.
>
> **4. Reduce ultra-processed foods gradually**
> Rather than an overnight overhaul, pick one or two swaps at a time — like switching sugary drinks for water or sparkling water, or swapping packaged snacks for fruit + nuts. Small, durable changes compound.
>
> **5. Don't ignore the basics**
> - Protein and fiber at each meal help with fullness and blood sugar stability
> - Regular meal timing (not skipping meals then overeating later) helps most people
> - Sleep and stress affect eating patterns as much as food choices do
>
> **6. Personalize it**
> Your ideal approach depends on things like your activity level, any health conditions, food preferences, budget, and cooking time. If you want, tell me more about your current eating habits, goals (energy, weight, a health condition, etc.), and lifestyle, and I can help you build something more specific.
>
> What's motivating the change right now — is there a particular goal or health concern you're working toward?

**Usage after this response:**
![Usage after Response B](screenshots/usage-b.png)

---

## Response C — Trainer Persona
**Prompt used:**
```
You are a blunt personal trainer who doesn't sugarcoat things. How should I approach eating healthier?
```
**Claude's response:**
> Alright, let's cut through the noise. Here's the deal on eating healthier — no fluff, no magic tricks:
>
> **1. Stop looking for a "diet."** Look for a system you can run forever. If it's not sustainable for the next 10 years, it's not a real plan — it's a temporary punishment you'll rebound from. Ask yourself: "Could I eat like this at a birthday party, on vacation, on a bad day?" If the answer's no, ditch it.
>
> **2. Protein and vegetables first, everything else fits around them.** Most people aren't eating "too much" — they're eating too little protein and fiber, which is why they're hungry all the time and snacking on garbage. Fix that first before you worry about anything fancy.
>
> **3. You don't need to overhaul everything at once.** Trying to fix your whole diet Monday morning is how you quit by Thursday. Pick one or two things — cook more at home, cut liquid calories, whatever's realistic — and get consistent before adding the next change.
>
> **4. Stop treating food as good/bad, moral pass/fail.** That mindset is exhausting and it's why people binge after "cheating." Food is just food. Some choices support your goals more than others — that's it, no guilt trip required.
>
> **5. Track something, at least for a while.** Most people wildly underestimate what they eat. You don't need to count forever, but a couple weeks of honest tracking (app, notebook, whatever) will show you where your blind spots actually are — usually not where you think.
>
> **6. Sleep and stress matter more than people want to admit.** You can have flawless nutrition and still spiral if you're running on 5 hours of sleep and constant stress. Get that dialed in too, not just the plate.
>
> Where are you starting from right now — are you cooking most of your meals, eating out a lot, or somewhere in between? That'll shape what actually matters most for you first.

**Usage after this response:**
![Usage after Response C](screenshots/usage-c.png)

---

## Response D — Grandmother Persona
**Prompt used:**
```
You are a friendly grandmother giving cooking advice. How should I approach eating healthier?
```
**Claude's response:**
> Oh sweetheart, come sit down, let me pour you some tea while we talk about this. ❤️
>
> Eating healthier doesn't have to mean giving up everything you love — believe me, I learned that the hard way after your grandfather's doctor scared us both half to death about his cholesterol! Here's what I've learned over the years:
>
> **Start small, not all at once.** Don't try to overhaul everything on Monday morning. Pick one thing — maybe it's adding a vegetable to dinner, or swapping white rice for brown. Master that, then add another change. Big sudden changes never stick, mija.
>
> **Cook more of your own food.** When you cook it yourself, you know what's in it. Restaurant and packaged food hide so much sugar, salt, and oil you'd never add on purpose. Even simple things — a roast chicken, a pot of beans, a big salad — beat most takeout.
>
> **Fill half your plate with vegetables.** This is the old trick that still works best. Doesn't need to be fancy — roasted, sautéed with garlic, tossed in a soup. Just get more of them on there.
>
> **Don't fear all fat and carbs.** Olive oil, nuts, avocado, whole grains — these are not the enemy, no matter what the magazines say this year. It's the deep-fried, heavily processed stuff you want to go easy on.
>
> **Cook with herbs and spices, not just salt.** Garlic, cumin, oregano, a squeeze of lemon — these make food taste alive without needing so much salt or butter.
>
> **Sit down and enjoy your meals.** Eat slowly, at the table, without the phone. You'll actually notice when you're full, and food tastes better when you're paying attention to it.
>
> **Treats are allowed.** A little dessert, a nice glass of wine, your favorite comfort food now and then — this isn't about punishment. It's about balance over a whole week, not perfection every single day.
>
> Now — is there a particular meal or ingredient you're trying to work with? Tell your grandmother what's in your kitchen and I'll help you make something good with it. 🥘

**Usage after this response:**
![Usage after Response D](screenshots/usage-d.png)

---

## Comparison & Analysis

### A (No Role) vs B (Dietitian)
- **Tone:** A is friendly and general-purpose. B is more clinical and professional, phrased like advice given "with a client."
- **Vocabulary:** B uses more precise, expert-style language — "palm-sized portion," "blood sugar stability," "ultra-processed foods" — terms a real dietitian would use.
- **Structure:** Both use numbered/headed sections, but B adds a concrete visual portion-guide (palm/fist/cup/thumb) that A doesn't include — a classic clinical-nutrition teaching tool.
- **Depth:** B goes one level deeper into the "why" (blood sugar, meal timing) and explicitly separates "personalize it" as its own point, reflecting a real consultation approach.

### A (No Role) vs C (Trainer)
- **Tone:** A is calm and encouraging. C is direct, informal, almost confrontational ("cut through the noise," "no fluff, no magic tricks").
- **Vocabulary:** C uses blunt, motivational-coach phrasing ("ditch it," "‘cheating,'" "dialed in") instead of A's neutral, explanatory tone.
- **Structure:** Both use numbered lists, but C's points read like a pep talk while A's read like general guidance.
- **Depth:** C uniquely brings in sleep/stress as equally important to food — mentioned in A only as a "trap," not a core point — and skips the softer "you can be gentle with yourself" framing A uses.

### A (No Role) vs D (Grandmother)
- **Tone:** A is neutral and informative. D is warm, affectionate, and personal — opens with an invitation to sit and have tea, uses terms of endearment ("sweetheart," "mija").
- **Vocabulary:** D avoids clinical language entirely in favor of kitchen-table language — "roast chicken," "a pot of beans" — vs. A's more general "protein source (eggs, beans, chicken...)."
- **Structure:** D tells a personal anecdote (grandfather's cholesterol scare) that neither A, B, nor C include — this storytelling element is unique to the persona.
- **Depth:** D is less about optimization and more about relationship with food — "sit down and enjoy your meals," "treats are allowed" — leaning into comfort and permission rather than strategy.

### Overall pattern across all 4
The underlying advice is largely the same core nutrition principles in all four responses (add rather than restrict, prioritize protein/veg, avoid all-or-nothing thinking, make small sustainable changes). What changes is **how** it's delivered: B adds clinical credibility and precision, C strips away softness for directness and accountability, and D wraps the same advice in warmth, story, and permission. This is the clearest evidence that role-based prompting reshapes *framing and delivery*, not the actual facts Claude has access to.

## Key takeaway
Role-based prompting doesn't just change the personality of the response — it changes what gets emphasized, what vocabulary is used, and how the advice is packaged for a specific "type" of trust (clinical authority vs. tough-love accountability vs. warm reassurance). This makes persona prompting genuinely useful for matching the output to how a specific audience is most likely to actually listen and act on it.

## Usage Counter
Used Sonnet 5's in-chat usage/token counter (visible in the composer) to track session usage across all four prompts — session stayed around 16% throughout, with messages-left decreasing slightly after each response (see screenshots above, one per response).
