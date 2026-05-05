# AGENTS.md
## Project Purpose
This repository is a Japanese landing page hero design assistant called "LP Hero Architect".
The goal is not to auto-generate entire low-quality landing pages.
The goal is to help users make high-quality, conversion-focused LP hero sections by answering structured questions.
The application should generate:
- hero design summary
- first-view layout
- headline and subheadline options
- CTA options
- image generation prompt
- Canva/Figma editing instructions
- Codex implementation instructions
- JSON output for future API integration
## Core UX Principle
The user should feel:
"選ぶだけで、LPの第一印象が決まる。"
Make the product intuitive, visual, and polished.
Avoid making it look like a plain business form.
## Design Direction
Use:
- premium SaaS design
- clean Japanese UI
- card-based selection
- subtle gradient background
- clear visual hierarchy
- generous spacing
- readable typography
- elegant output panels
Avoid:
- cluttered forms
- cheap dashboard look
- too many borders
- dark unreadable UI
- randomly generated visual noise
## Technical Stack
Use:
- Next.js App Router
- TypeScript
- Tailwind CSS
- shadcn/ui if already configured or easy to add
- localStorage for saving projects
- no external API for MVP
## Implementation Rules
- Keep data definitions in lib/options.ts and lib/samples.ts
- Keep generation logic in lib/generator.ts
- Keep types in lib/types.ts
- Keep UI components small and readable
- Do not hard-code everything inside app/page.tsx
- Make the app easy to extend with an AI API later
## Output Quality Rules
The generated image prompt must be practical and usable.
Always include:
- clean negative space for headline and CTA
- no readable text inside the image
- no logos
- no real brand names
- no watermark
- premium commercial landing page quality
- strong visual hierarchy
- implementation-friendly composition
The generated implementation instruction must explain:
- layout structure
- responsive behavior
- image/text separation
- CTA placement
- component structure
- accessibility considerations
## Completion Criteria
Before finishing:
- run lint if available
- run build if available
- verify the page works in desktop and mobile widths
- verify sample projects load
- verify copy buttons work
- verify output changes when selections change
- verify no important UI is broken
