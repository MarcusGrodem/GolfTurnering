# Hjemmebane Brand Identity

## Brand Idea

**Hjemmebane** connects three meanings: playing on a golf course, returning to the Stavanger region, and meeting employers in an environment where students can feel at home.

The visual identity should feel **grounded, sociable, and ambitious**. It should be recognizably golf-related without relying on a generic golf ball, crossed clubs, shield, or luxury country-club styling.

## Recommended Direction: Kystfairway

Kystfairway combines the green structure of the course with a restrained coastal reference. The identity is light and useful during daytime, while the red flag accent gives calls to action and tournament moments clear energy.

### Core Colors

| Token | Preview | Hex | OKLCH target | Use |
|---|---|---|---|---|
| Fairway | ![Fairway](https://placehold.co/320x120/18543F/18543F.png) | `#18543F` | `oklch(41% 0.09 159)` | Primary brand, navigation, buttons |
| Scorecard | ![Scorecard](https://placehold.co/320x120/F4F6F0/F4F6F0.png) | `#F4F6F0` | `oklch(97% 0.01 135)` | Main background |
| Ink | ![Ink](https://placehold.co/320x120/17231E/17231E.png) | `#17231E` | `oklch(24% 0.02 155)` | Text and dark surfaces |
| Flag | ![Flag](https://placehold.co/320x120/DC604D/DC604D.png) | `#DC604D` | `oklch(63% 0.16 31)` | Registration, countdown, key highlights |
| Fjord | ![Fjord](https://placehold.co/320x120/7FA9B2/7FA9B2.png) | `#7FA9B2` | `oklch(70% 0.06 210)` | Information, secondary graphic fields |
| Medal | ![Medal](https://placehold.co/320x120/D1A647/D1A647.png) | `#D1A647` | `oklch(73% 0.12 84)` | Awards and result highlights only |

Use Scorecard and Ink for most of the interface, Fairway for structure, and Flag sparingly for important action. Fjord and Medal are supporting colors, not competing primary colors. Avoid gradients.

### Interface Tokens

```css
:root {
  --color-brand: oklch(41% 0.09 159);
  --color-brand-hover: oklch(35% 0.08 159);
  --color-surface: oklch(97% 0.01 135);
  --color-surface-raised: oklch(99% 0.005 135);
  --color-ink: oklch(24% 0.02 155);
  --color-muted: oklch(49% 0.025 155);
  --color-border: oklch(86% 0.018 155);
  --color-action: oklch(63% 0.16 31);
  --color-info: oklch(70% 0.06 210);
  --color-award: oklch(73% 0.12 84);
}
```

Final values must be contrast-tested in actual components. Flag is suitable for filled calls to action with dark Ink text only after contrast verification; use Fairway for the default primary button.

## Typography

### Display: Bricolage Grotesque

Use for the logo wordmark, page titles, countdown numerals, tournament results, and short campaign headlines. Its slightly irregular construction gives Hjemmebane a social event character without becoming childish.

- Headings: weights 600–700.
- Wordmark: weight 700.
- Do not use for long body copy.
- Keep letter spacing at `0`.

### Body and Interface: Archivo

Use for navigation, body text, profiles, forms, tables, labels, and buttons. It is compact enough for operational screens but still feels editorial and human.

- Body: weight 400.
- Interface labels and buttons: weight 600.
- Dense tables: weight 400–500.
- Use tabular numerals for scores, handicaps, times, and countdowns.

Both families are available from [Google Fonts](https://fonts.google.com/). Self-host production font files when practical to improve privacy and loading control.

## Logo System

### Primary Mark: Home Flag

The working mark is an `H` built from two course boundaries and a central crossbar. The right stem becomes a flagpole with a Flag-red pennant. This gives three readings without adding detail:

- `H` for Hjemmebane.
- A golf flag and fairway.
- Two sides meeting on common ground, reflecting student-company connection.

Working assets:

- `brand/hjemmebane-mark.svg` — symbol for avatars, favicon, social media, and compact navigation.
- `brand/hjemmebane-lockup.svg` — horizontal symbol and wordmark.
- `brand/hjemmebane-lockup-reverse.svg` — light version for Fairway or Ink backgrounds.

The lockup is a working digital master. Before print production, convert the approved wordmark to vector outlines in a design tool so it does not depend on an installed font.

### Clear Space and Minimum Size

- Keep clear space equal to the width of the flag around the full logo.
- Minimum mark size: `24px` digital or `8mm` print.
- Minimum horizontal lockup width: `140px` digital or `35mm` print.
- Never rotate, outline, stretch, add shadows, or recolor individual elements outside the approved versions.

## Iconography

Use **Lucide** icons in the website interface with a consistent `1.75px` stroke. Icons should clarify actions, not decorate headings.

Recommended mappings:

| Function | Lucide icon |
|---|---|
| Tournament | `Flag` |
| Program | `CalendarDays` |
| Sponsors | `Handshake` |
| Profile | `CircleUserRound` |
| Student | `GraduationCap` |
| Company | `Building2` |
| Handicap or score | `Gauge` |
| Team | `UsersRound` |
| Location | `MapPin` |
| CV/document | `FileText` |
| Favorite | `Star` |
| Contact | `Mail` |
| Language | `Languages` |

Use filled Flag color only for selected favorites or critical event actions. Do not place every icon inside a colored rounded square.

## Photography

Photography should show the actual course, participants, company representatives, and social moments. Prefer bright summer daylight, visible faces with consent, honest golf action, and wide course context. Avoid dark stock photography, staged handshake close-ups, heavy filters, and blurred atmospheric images.

The first viewport should use a strong Sola GK image when usage rights are confirmed. Until then, use a clearly marked placeholder rather than unrelated stock imagery.

## Graphic Language

- Use thin scorecard rules and course-map-like lines to structure information.
- Use the flag shape as a small directional device for deadlines and live status.
- Use large tabular numbers for countdown and scoring.
- Keep cards at `8px` radius or less and reserve them for profiles, sponsor entries, and tools.
- Sponsor tickers should be monochrome by default and reveal original logo colors on hover or focus, subject to sponsor agreements.
- Motion should be restrained: steady sponsor movement, clear countdown changes, and short state transitions with reduced-motion support.

## Voice

Hjemmebane should sound direct, welcoming, and capable.

- Prefer: “Møt bedriftene på banen.”
- Prefer: “Finn laget ditt.”
- Prefer: “Vil dere være med på hjemmebane?”
- Avoid inflated claims about careers, exclusivity, or guaranteed recruitment outcomes.
- Avoid overly formal golf language that makes first-time tournament players feel unwelcome.

## Decision Before Build

Test the identity on four realistic views before treating it as final:

1. Public homepage with Sola GK image, countdown, and sponsor ticker.
2. Student profile and payment flow.
3. Company student-discovery view.
4. Mobile event-day program and results view.

The final logo should also be checked at favicon size, embroidered on a cap, printed on a scorecard, and placed beside sponsor logos.
