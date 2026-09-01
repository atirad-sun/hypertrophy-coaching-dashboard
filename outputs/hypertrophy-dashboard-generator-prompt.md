# Prompt: Generate the Hypertrophy Coaching Dashboard

You are an expert product designer and front-end engineer. Read the companion file `hypertrophy-coaching-context.md` completely before generating anything. Treat it as the source of truth for the user's profile, coaching guidance, content, and visual requirements.

Create a polished, self-contained, responsive HTML dashboard that makes the coaching plan easy to understand and follow week to week.

## Output contract

- Return one complete `index.html` file only, inside a single HTML code block.
- Use semantic HTML, modern CSS, and vanilla JavaScript. No build step and no framework.
- Keep all CSS and JavaScript inline. Do not require a backend or external assets.
- The page must work on mobile and desktop, with touch-friendly controls and accessible labels.
- Use a calm, premium training-journal aesthetic: dark charcoal base, warm off-white text, restrained amber/lime accents, clear cards, generous spacing, and strong typographic hierarchy.
- Avoid fake data, unsupported medical claims, excessive decoration, and information overload.
- Make the page usable without JavaScript; JavaScript may enhance tabs, accordions, checklists, and progress inputs.
- Include responsive behavior, visible keyboard focus states, sufficient color contrast, reduced-motion support, and appropriate ARIA attributes.

## Information architecture

Build the page in this order:

1. Header: title, short positioning statement, and a clear “Start here” action.
2. Current snapshot: age, height, weight, goal, training availability, and physique priorities.
3. “The plan in one glance”: recomposition goal, calorie experiment, protein target, weekly lifting frequency, cardio, sleep, and tracking.
4. Weekly execution view: an easy 3–4-day rotation showing Upper A, Lower A, Upper B, Lower B, plus cardio placement. Explain that the user can continue the rotation across weeks when only three days are available.
5. Workout detail: exercise tables/cards with sets, reps, effort target, rest guidance, substitutions, and progression notes.
6. Nutrition dashboard: protein target, calorie starting range, expected rate of loss, plate/meal rules for eating out, and whey guidance.
7. Recovery and DOMS: sleep target, warm-up/intensity guidance, what normal soreness looks like, and when to reduce or change an exercise.
8. Progress tracker: editable or printable weekly fields for average weight, waist, photos, performance, protein/calories, sleep, soreness, and notes. Include the adjustment rules.
9. A compact “rules to remember” section and a safety note encouraging professional advice for pain, injury, or medical concerns.

## Interaction requirements

- Use tabs or segmented controls for the four workout days if that improves scanability.
- Use collapsible sections for exercise substitutions, DOMS guidance, and eating-out tactics.
- Include a simple weekly checklist with non-persistent checkboxes.
- Include a small “How to progress” visual or step sequence showing double progression and 1–3 RIR.
- Do not pretend that entries are saved unless localStorage is actually implemented. If localStorage is used, label it clearly.

## Content rules

- Preserve the coaching details and numerical targets from `hypertrophy-coaching-context.md`.
- Use plain language and explain jargon briefly, especially RIR, double progression, recomposition, and DOMS.
- Show the distinction between a starting experiment and a fixed prescription: calories and adjustments are validated using 2–3 weeks of morning weigh-ins.
- Keep the dashboard actionable: every major section should answer “What do I do?”
- Do not invent an exact body-fat percentage, maintenance calorie number, injury diagnosis, or guaranteed outcome.
- Do not turn soreness into a test of workout quality.

Before finalizing, check that every section in the context file is represented, the page is coherent at 375px wide, and the HTML is valid and self-contained.
