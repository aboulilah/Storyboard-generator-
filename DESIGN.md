---
name: Kinetic Narrative
colors:
  surface: '#11131b'
  surface-dim: '#11131b'
  surface-bright: '#373942'
  surface-container-lowest: '#0c0e16'
  surface-container-low: '#191b23'
  surface-container: '#1d1f27'
  surface-container-high: '#282a32'
  surface-container-highest: '#32343d'
  on-surface: '#e1e2ed'
  on-surface-variant: '#c3c6d7'
  inverse-surface: '#e1e2ed'
  inverse-on-surface: '#2e3039'
  outline: '#8d90a0'
  outline-variant: '#434655'
  surface-tint: '#b4c5ff'
  primary: '#b4c5ff'
  on-primary: '#002a78'
  primary-container: '#2563eb'
  on-primary-container: '#eeefff'
  inverse-primary: '#0053db'
  secondary: '#d0bcff'
  on-secondary: '#3c0091'
  secondary-container: '#571bc1'
  on-secondary-container: '#c4abff'
  tertiary: '#ffb596'
  on-tertiary: '#581e00'
  tertiary-container: '#bc4800'
  on-tertiary-container: '#ffede6'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#dbe1ff'
  primary-fixed-dim: '#b4c5ff'
  on-primary-fixed: '#00174b'
  on-primary-fixed-variant: '#003ea8'
  secondary-fixed: '#e9ddff'
  secondary-fixed-dim: '#d0bcff'
  on-secondary-fixed: '#23005c'
  on-secondary-fixed-variant: '#5516be'
  tertiary-fixed: '#ffdbcd'
  tertiary-fixed-dim: '#ffb596'
  on-tertiary-fixed: '#360f00'
  on-tertiary-fixed-variant: '#7d2d00'
  background: '#11131b'
  on-background: '#e1e2ed'
  surface-variant: '#32343d'
typography:
  display-lg:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  title-md:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '500'
    lineHeight: 24px
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-md:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
  mono-label:
    fontFamily: JetBrains Mono
    fontSize: 11px
    fontWeight: '500'
    lineHeight: 14px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 40px
  gutter: 16px
  margin: 24px
  sidebar-width: 280px
---

## Brand & Style

The design system is engineered for a high-utility storyboard generation platform. It balances the precision of a professional productivity tool with the spark of creative exploration. The brand personality is **efficient, inspiring, and professional**, designed to disappear behind the user's content while providing a rigid, reliable framework for visual storytelling.

The design style is **Corporate Modern with a subtle leaning toward Minimalism**. It prioritizes high information density and legibility, using deep neutrals to ground the interface and vibrant accents to guide the user's focus toward generative actions. The goal is to evoke a sense of focused "flow state" for directors, writers, and artists.

## Colors

The palette is anchored in a dark-mode-first architecture to reduce eye strain during long creative sessions and to make storyboard frames "pop" against the UI.

- **Primary (Action Blue):** A high-energy blue used exclusively for primary calls-to-action, generation buttons, and active states.
- **Secondary (Creative Purple):** Used for secondary features like "Remix," "Iterate," or tagging—actions that represent the creative spark.
- **Neutrals:** A range of deep slates and charcols. The background uses the darkest slate to provide depth, while surface containers use slightly lighter tones to establish hierarchy.
- **Functional:** Success, Warning, and Error colors are desaturated to maintain the professional aesthetic, only gaining vibrancy when user attention is required.

## Typography

The design system utilizes **Inter** for all UI elements to ensure maximum legibility and a sharp, modern feel. The hierarchy is strictly enforced to manage complex metadata (shot numbers, camera angles, timestamps) alongside user-generated scripts.

- **Headlines:** Use tighter letter-spacing and heavier weights to create a strong visual anchor.
- **Body:** Optimized for readability in multi-line scene descriptions.
- **Labels:** Small-cap or bolded utility text is used for "Shot Type" or "Frame ID" to differentiate system metadata from creative content.
- **Mono:** An optional monospace font (like JetBrains Mono) is used specifically for frame coordinates or technical export settings.

## Layout & Spacing

This design system uses a **12-column fluid grid** for the main workspace, with a **fixed left-hand navigation/utility bar**. 

- **Layout Model:** A three-pane architecture is preferred: Tools (Left, fixed), Canvas (Center, fluid), and Properties/Assets (Right, collapsible).
- **Rhythm:** An 8px linear scale (with a 4px half-step for tight components) ensures a mathematical, engineered feel. 
- **Responsive Behavior:** 
  - **Desktop:** Full 3-pane view.
  - **Tablet:** Right properties panel collapses into a bottom sheet or modal. 
  - **Mobile:** Single-column view focusing on the "Frame Preview" with a bottom navigation bar for quick tool access.

## Elevation & Depth

Hierarchy is established through **Tonal Layering** supplemented by subtle ambient shadows. 

- **Level 0 (Background):** The darkest slate (#0F172A). No shadow.
- **Level 1 (Panels):** Slightly lighter (#1E293B). Defines the workspace and sidebars.
- **Level 2 (Cards/Frames):** Surface color with a 1px border (#334155) and a very soft, 12% opacity black shadow with a 4px blur.
- **Level 3 (Modals/Popovers):** Higher contrast with a 24% opacity shadow and a 16px blur to lift the element significantly off the canvas.

Avoid heavy skeuomorphism; depth should feel clinical and intentional, like stacked sheets of acetate on a lightbox.

## Shapes

The shape language is consistently **Rounded**, using an 8px (0.5rem) base to soften the technical nature of the interface.

- **Buttons & Inputs:** Use the 8px base (rounded-md).
- **Cards & Storyboard Frames:** Use 16px (rounded-lg) to create a distinct frame for the visual content within.
- **Chips & Tags:** Use 32px (rounded-full/pill) to distinguish them from actionable buttons or interactive inputs.

## Components

- **Buttons:** Primary buttons are solid "Action Blue" with white text. Secondary buttons use a ghost style (Action Blue border and text) or solid "Creative Purple" for specific creative features.
- **Chips:** Used for "Scene Tags" or "Character Filters." These should have a subtle background tint (15% opacity of the secondary color) and a 1px solid border.
- **Inputs:** Dark field fills (#0F172A) with a 1px slate border. Focus state should trigger an "Action Blue" border glow.
- **Storyboard Cards:** The hero component. Features a large aspect-ratio image area at the top, a "Shot ID" label in the top-left, and a script text area at the bottom.
- **Timeline/Filmstrip:** A specialized horizontal list at the bottom of the screen using the Level 1 surface color to allow users to scrub through the generated sequence.
- **Progress Indicators:** Linear, thin bars using the Primary-to-Secondary gradient to represent AI generation progress.