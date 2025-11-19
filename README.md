# Better Feedback Survey Form

A responsive survey form for collecting feedback from creators, builders, and hustlers.  
This fulfills the freeCodeCamp **Survey Form** project requirements, but with copy tailored to your Better Endeavor / “trailblazer” branding.

---

## Overview

The page contains:

- Title: **“Better Feedback, Better Vibes”**
- Description explaining the purpose of the survey.
- Form fields:
  - Name (required)
  - Email (required, with email validation)
  - Age (optional number between 13 and 100)
  - Role / current hustle (select dropdown)
  - Recommendation rating (radio buttons)
  - Interests (checkboxes, multi-select)
  - Open-text feedback textarea
- A full-width submit button: **“Send It ✨”**

No JavaScript is required; the form is focused on semantic HTML and clean CSS.

---

## Form Fields

1. **Name**  
   - `type="text"`, required  
   - `id="name"` for FCC tests

2. **Email**  
   - `type="email"`, required  
   - `id="email"`

3. **Age**  
   - `type="number"` with `min="13"` and `max="100"`  
   - `id="number"`

4. **Role / Current Hustle**  
   - `<select id="dropdown">` with options like:
     - Student
     - Freelancer
     - Startup/Creator
     - Other

5. **Recommendation** (radio group)  
   - “Absolutely!”  
   - “Maybe, needs some tweaks.”  
   - “Nah, not my vibe.”

6. **Interests** (checkbox group)  
   - Vending & Passive Income  
   - Web Dev & SaaS Projects  
   - Gaming & Streaming  
   - Branding & Creative Strategy  

7. **Comments**  
   - `<textarea id="comments">` for open feedback.

The form uses labels correctly tied to inputs, and `fieldset` + `legend` for grouped questions.

---

## Styling

Core styling is in `styles.css`:

- Centered layout with `max-width: 700px` and `margin: auto`.
- Light grey background (`#f4f6fa`) with white form card.
- Soft drop shadow and rounded corners for the form.
- Segoe UI font across the page.
- Accent colors:
  - Heading: `#FF6B81`
  - Label text: `#243B73`
  - Button: `#FFD93D` (hover → `#00C2D1` with white text)

Inputs and textarea are full-width, with consistent padding and border-radius.

---

## How to Use

1. Open the page in your browser.
2. Fill out the fields (name + email required).
3. Click **Send It ✨** to submit.

Currently the form doesn’t post to a backend; you can hook it up later to:

- An email service (Formspree, Netlify Forms, etc.), or
- Your own API endpoint.

---

## Project Structure

```text
survey-form/
├── index.html   # Survey structure, labels, inputs, fieldsets
└── styles.css   # Layout, colors, typography, button states
What I Practiced
Semantic HTML form structure (labels, fieldsets, legends).

Accessible input labelling and grouping.

Basic validation with HTML attributes (required, min, max, type="email").

Responsive, centered card layout with clean visual hierarchy.

Future Improvements
Add client-side validation + success/error messages.

Integrate with a backend to store responses.

Add small animations or success toast on submit.

Add optional “Other” text field when certain choices are selected.

Author
Created by Trevyn Sanders.