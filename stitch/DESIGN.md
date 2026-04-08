```markdown
# Design System Document: Professional Aesthetic Clinic

## 1. Overview & Creative North Star: "The Human Canvas"
The digital experience for this clinic must bridge the gap between clinical precision and human warmth. Our Creative North Star is **"The Human Canvas."** We treat the interface not as a software grid, but as an organic, layered composition that mirrors the care and intentionality of an aesthetic treatment.

To move beyond the "generic template" look, this design system rejects rigid containers and harsh separators. Instead, it utilizes **Asymmetric Breathing Room**—where whitespace isn't just "empty," but an active structural element that guides the eye. We favor tonal depth over flat surfaces, ensuring the clinic feels approachable to the local community in Resistencia while maintaining a high-end, professional authority.

---

## 2. Colors & Surface Logic
The palette is grounded in warm neutrals and earth-toned accents, moving away from "medical blue" or "sterile white" toward a more "skin-adjacent" spectrum.

### The Color Roles
*   **Primary (Terracotta - `#8b4e37`):** Use for high-intent actions and brand-defining moments.
*   **Secondary (Sage - `#536346`):** Use for calming elements, health-related information, and secondary CTAs.
*   **Surface Hierarchy:** Our "White" is never pure white; we use `surface` (`#fcf9f4`) as the base to keep the screen from feeling cold.

### The "No-Line" Rule
**Explicit Instruction:** Designers are prohibited from using 1px solid borders to define sections or containers. 
*   **Separation via Tone:** Boundaries must be defined solely through background color shifts. For example, a card should be `surface-container-lowest` sitting on a `surface-container-low` background. 
*   **The Signature Glow:** For primary CTAs, use a subtle linear gradient from `primary` (`#8b4e37`) to `primary-container` (`#d58b70`). This adds "soul" and a soft inner-glow that flat colors lack.

### Glassmorphism & Texture
Floating elements (modals, navigation bars) should utilize a "Frosted Glass" effect. Use the `surface` color at 80% opacity with a `backdrop-blur` of 12px-20px. This allows the warm tones of the content beneath to bleed through, creating an integrated, premium feel.

---

## 3. Typography: The Editorial Voice
We use typography to establish trust. The mix of a geometric heading and a legible body font creates a "Professional Editorial" vibe.

*   **Display & Headlines (Manrope):** This is our "Expert Voice." Use `display-lg` (3.5rem) for hero statements. The modern, slightly rounded geometry of Manrope feels high-tech but remains friendly.
*   **Body & Titles (Work Sans):** This is our "Consultant Voice." Work Sans provides exceptional legibility at smaller scales. Use `body-lg` (1rem) for treatment descriptions to ensure clients never struggle to read professional advice.
*   **Hierarchy Note:** Always maintain a high contrast between headings and body text. If a headline is `headline-lg`, the supporting text should be `body-md` to ensure the information feels curated, not cluttered.

---

## 4. Elevation & Depth: Tonal Layering
Traditional drop shadows are too "digital." To achieve a premium, physical feel, we use **Tonal Layering.**

### The Layering Principle
Think of the UI as stacked sheets of fine, heavy-weight paper. 
1.  **Level 0 (Base):** `surface` (`#fcf9f4`)
2.  **Level 1 (Sections):** `surface-container-low` (`#f6f3ee`)
3.  **Level 2 (Interactive Cards):** `surface-container-lowest` (`#ffffff`)

### Ambient Shadows
When a component must float (e.g., a "Book Appointment" floating button), use an **Ambient Shadow**:
*   **Blur:** 24px - 40px.
*   **Opacity:** 6%.
*   **Color:** Derived from `on-surface` (`#1c1c19`). This creates a natural "lift" rather than a dark, artificial shadow.

### The "Ghost Border" Fallback
If accessibility requirements demand a border (e.g., in high-contrast modes), use the **Ghost Border**: `outline-variant` (`#d8c2bb`) at 20% opacity. Never use 100% opaque borders.

---

## 5. Components

### Buttons
*   **Primary:** Pill-shaped (`full` roundedness). Background: `primary` gradient. Text: `on-primary` (`#ffffff`). Use `xl` padding for a substantial, "touchable" feel.
*   **Secondary:** Pill-shaped. Background: `surface-container-highest`. Text: `on-surface`.
*   **Interaction:** On hover, the button should not just change color; it should "lift" slightly using an Ambient Shadow.

### Cards & Lists
*   **Requirement:** No divider lines. 
*   **Separation:** Use `0.75rem` (md) roundedness for cards. Separate list items using vertical whitespace (e.g., `1.5rem` between items) and subtle background shifts.
*   **Content:** Treat cards as mini-compositions with intentional padding (minimum `2rem`).

### Input Fields
*   **Style:** Do not use "boxed" inputs. Use a soft-filled style using `surface-container-highest`. 
*   **Focus State:** The background shifts to `surface-container-lowest` with a subtle `primary` (Terracotta) "Ghost Border" at 40% opacity.

### Selection Chips
*   Used for selecting treatment categories. Use `secondary-container` (`#d6e9c3`) for active states to introduce the "Sage" accent, signaling a "natural/selected" state.

---

## 6. Do's and Don'ts

### Do:
*   **Do** use asymmetrical layouts. Place an image slightly off-center to break the "template" feel.
*   **Do** prioritize "Real Client" imagery. The clinic is professional and close to people—avoid overly airbrushed stock photos.
*   **Do** use the `lg` (1rem) and `xl` (1.5rem) roundedness for large containers to soften the clinical feel.

### Don't:
*   **Don't** use 1px dividers. If you feel the need for a line, use a 24px gap of whitespace instead.
*   **Don't** use pure black (`#000000`). Always use `on-surface` (`#1c1c19`) for text to maintain the warm, professional tone.
*   **Don't** crowd the screen. If a section feels "full," double the margin. Professionalism is shown through the luxury of space.
*   **Don't** use flat design. Every element should feel like it has a weight and a place in a physical stack.

---

**Director's Final Note:** 
In Resistencia, the climate and culture are warm and communal. This design system should feel like stepping into a well-lit, air-conditioned clinic: a relief, a place of expert care, and above all, a space designed for the human touch. Stick to the tonal layering—let the colors do the structural work, and let the typography provide the authority.```