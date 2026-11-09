---
name: no-ai-slop
description: Universal standard to eliminate robotic AI copy, developer jargon in UI, redundant subtitles, affirmation badges, and tacky neon glows, while enforcing tactile, feedback-driven motion across hovers, taps, tabs, toggles, and state transitions. Use when writing, reviewing, or refactoring user-facing text, micro-interactions, animations, and UI styles.
---

# No AI Slop: Universal UI Copy and Motion Standard

This skill eliminates the predictable, low-craft hallmarks of AI-generated frontends across all software categories (SaaS, consumer apps, e-commerce, developer tools, and productivity software):
- Robotic copy and database-query phrasing.
- Redundant subtitles that state the obvious under every single title or button.
- Developer jargon and file format lists masquerading as user interface text.
- Self-congratulatory status affirmations and operational badges.
- Tacky neon hover glows, colored shadow halos, and dead, lifeless CSS transitions.

Other skills handle backend architecture and database schemas. This skill is strictly focused on **UI copy craft** and **tactile, feedback-driven interaction motion**.

---

## 1. Eliminate Status Affirmations and Proof-of-Work Badges

AI agents have a reflexive habit of adding operational badges and status text to confirm their backend wiring works. Unless the product is an infrastructure uptime dashboard, users assume an interface is working until told otherwise.

### Anti-Patterns Across Different Domains

#### SaaS and Account Settings
- **AI Slop**: A card labeled `"Stripe Payment Gateway"` with a green badge `"Operational"` and text `"Webhook listeners verified in real-time."`
- **Clean UI**: `"Payment method"` with `"Card ending in 4242"` and an `"Edit"` button.

#### Cloud and Data Management
- **AI Slop**: A sync row labeled `"Cloud Data Persistence Engine"` with badge `"Active Sync Thread"`.
- **Clean UI**: `"Saved"` or `"Synced 2m ago"`.

#### Service and Integration Cards
- **AI Slop**: `"Active Analytics Engine"`, `"Live Pipeline Thread"`, or badges saying `"Telemetry Live: High Throughput"`.
- **Clean UI**: Plain integration name (`"Google Analytics"` or `"Slack"`), with a subtle connection dot or checkmark.

#### General Consumer UI
- **AI Slop**: `"Preferences successfully committed to persistent local storage."`
- **Clean UI**: Silent auto-save, or a quiet 1-second checkmark icon.

---

## 2. The Jargon-to-Human Translation Table

AI agents default to the vocabulary of backend documentation, API specs, and database schemas. Normal human beings speak in plain, everyday language.

### General Settings and Appearance

| AI Slop Copy | Human Friendly UI Text |
| :--- | :--- |
| Configure client viewport appearance theme | Theme |
| Select your visual theme or sync automatically with your system preference | (Delete subtitle entirely) |
| Synchronize with host operating system visual preference | System |
| Adjust base typography rendering scale | Text size |
| Adjust the base typography size for readable content display | (Delete subtitle entirely) |
| Toggle interface layout density compression | Compact mode |
| User profile identification handle | Name |

### Files, Media, and Attachments

AI models frequently dump file format acronyms into user-facing buttons and cards:

| AI Slop Copy | Human Friendly UI Text |
| :--- | :--- |
| Ingest multimodal image payload from filesystem | Upload image |
| Attach PNG, JPG, WEBP, or GIF visual media | (Delete subtitle entirely) |
| Ingest plaintext or source code document payload | Upload document / Upload file |
| Attach PDF, TXT, DOCX, or code source files | (Delete subtitle entirely) |
| Execute persistent cache purge operation | Clear cache |
| Export database records as structured JSON payload | Export data |
| Permanently drop designated record from datastore | Delete |

### Billing, Commerce, and Subscriptions

| AI Slop Copy | Human Friendly UI Text |
| :--- | :--- |
| Execute payment transaction processing pipeline | Pay now |
| Configure recurring billing invoice payment tier | Subscription plan |
| Select destination fulfillment logistics method | Shipping method |
| Active item collection inventory | Your cart / Your bag |
| Apply promotional deduction token code | Promo code |

### Search, Networking, and APIs

| AI Slop Copy | Human Friendly UI Text |
| :--- | :--- |
| Trigger automated web retrieval pipeline | Search web |
| Query database entity records | Search |
| Establish authenticated websocket handshake | Connecting... |
| Inbound payload transmission failed | Connection error |
| Re-initialize default application parameters | Reset to defaults |
| View persisted user event logs | Activity history |

---

## 3. The Subtitle Killer: Kill Stating the Obvious

The most pervasive AI UI slop is appending an explanatory descriptive sentence under every single header, card, input, and menu option.

### The Self-Evidence Rule
Ask: **"Does a regular human already know what this control does from the title alone?"**
If yes, the subtitle is slop. Delete it immediately.

### Multi-Domain Examples

#### Example A: Settings Sections (Theme, Display, Audio)
- **AI Slop**:
  ```html
  <div>
    <h3>Appearance Theme</h3>
    <p>Select your visual theme or sync automatically with your system preference.</p>
    <div class="theme-options">
      <button>Light</button>
      <button>Dark</button>
      <button>System</button>
    </div>
  </div>
  ```
- **Clean UI**:
  ```html
  <div>
    <h3>Theme</h3>
    <div class="theme-options">
      <button>Light</button>
      <button>Dark</button>
      <button>System</button>
    </div>
  </div>
  ```

#### Example B: Media and Attachment Modals or Menus
- **AI Slop**:
  ```html
  <button>
    <UploadIcon />
    <div>
      <div>Upload Image</div>
      <p>Attach PNG, JPG, WEBP, or GIF visual media</p>
    </div>
  </button>
  <button>
    <DocumentIcon />
    <div>
      <div>Upload Document</div>
      <p>Attach PDF, TXT, DOCX, or code source files</p>
    </div>
  </button>
  ```
- **Clean UI**:
  ```html
  <button>
    <UploadIcon />
    <span>Upload image</span>
  </button>
  <button>
    <DocumentIcon />
    <span>Upload document</span>
  </button>
  ```

#### Example C: Form Inputs (E-Commerce or Auth)
- **AI Slop**:
  ```html
  <label>Shipping Address</label>
  <p class="subtitle">Please provide the physical geographical location where you want your order delivered.</p>
  <input type="text" />
  ```
- **Clean UI**:
  ```html
  <label>Shipping address</label>
  <input type="text" placeholder="123 Main St, Apt 4B" />
  ```

#### Example D: Action Menus and Dropdowns
- **AI Slop**:
  ```html
  <div class="menu-item">
    <span>Copy Link</span>
    <small>Copy the unique URL of this item to your system clipboard for sharing.</small>
  </div>
  ```
- **Clean UI**:
  ```html
  <div class="menu-item">
    <span>Copy link</span>
  </div>
  ```

---

## 4. Eliminate Nested Header Redundancy

AI models love nesting repetitive titles inside containers:
- Page Header: `"Team Management"`
- Section Card: `"Team Members"`
- Table Header: `"Team Member Roster"`
- Subhead: `"List of current team members in your organization"`

### The Rule
Never repeat parent nouns in child sections.
- Page Header: `"Team"`
- Section: (No redundant subhead needed, table column names speak for themselves: `"Member"`, `"Role"`, `"Access"`).

---

## 5. Ban Tacky Glows and Generic Slop: The Universal Motion and Interaction Standard

AI interfaces fail in one of two opposite directions:
1. **Neon Glow Slop**: Cheap, over-saturated colored drop-shadow halos (`hover:shadow-rose-500/50`, `drop-shadow-[0_0_12px_...]`), pulsating outline rings (`animate-pulse ring-primary/50`), and blurry neon focus halos.
2. **Dead, Generic CSS Slop**: Slapping `transition: all 0.2s ease` with flat gray background swaps, instant 0ms tab cuts, harsh linear loaders, and lifeless non-reactive buttons.

Great software (Apple iOS/macOS, Linear, Stripe, Raycast) does not use neon halos, and it is **never static, flat, or boring**. It feels alive because every interaction has **tactile feedback, physical momentum, spring tension, and organic deceleration**.

### Strictly Banned Slop Patterns
- **Colored Shadows and Neon Halos**:
  - `hover:shadow-[0_0_20px_rgba(225,29,72,0.5)]` (BANNED)
  - `hover:drop-shadow-[0_0_12px_rgba(59,130,246,0.6)]` (BANNED)
  - `hover:shadow-rose-500/40`, `hover:shadow-indigo-500/40` (BANNED)
- **Colored Background Overrides on Neutral Controls**:
  - Tinting neutral sliders, dividers, or scrollbars with saturated brand colors on drag or hover (BANNED).
- **Pulsating Outline Halos**:
  - `animate-pulse ring-2 ring-primary/50` on resting buttons or badges (BANNED).
- **Dead, Lifeless Wireframe Hovers and Instant Cuts**:
  - `hover:bg-zinc-100 transition-colors` with generic linear easing and zero physical press response (AVOID).
  - Instant 0ms background snap on tab or filter switches (AVOID).

---

### The Tactile, Feedback-Driven Interaction System

Every interaction in the UI must provide physical, kinetic feedback matched to the user's intent:

#### 1. Tactile Switch Compression (Active Press and Tap)
Interactive buttons, chips, and cards must physically compress when clicked or tapped, mimicking the mechanical resistance of a physical switch:
```css
.tactile-btn {
  transition: transform 0.12s cubic-bezier(0.2, 0.9, 0.3, 1), background-color 0.15s ease, color 0.15s ease;
}
.tactile-btn:active {
  transform: scale(0.96);
}
```
In Tailwind:
```html
<button class="transition-all duration-150 ease-out active:scale-[0.96] hover:bg-zinc-100 dark:hover:bg-zinc-800">
  Save
</button>
```

#### 2. Kinetic Surface Lift (Hover Elevation and Surface Tension)
Instead of glowing with neon colors, interactive cards and modules physically elevate toward the user on hover with subtle vertical float and tightening elevation shadow:
```html
<div class="rounded-2xl border border-zinc-200/80 bg-white p-5 shadow-xs transition-all duration-200 cubic-bezier(0.16, 1, 0.3, 1) hover:-translate-y-0.5 hover:border-zinc-300 hover:shadow-md dark:border-zinc-800 dark:bg-zinc-900 dark:hover:border-zinc-700">
  ...
</div>
```

#### 3. Directional Vector Momentum (Chevrons, Links, and Affordances)
Interactive icons lead the user's eye by shifting slightly along their axis of motion on hover:
- **Forward Action (Arrow / Next)**:
  ```html
  <button class="group flex items-center gap-2">
    <span>View reports</span>
    <IconArrowRight class="transition-transform duration-150 ease-out group-hover:translate-x-1" />
  </button>
  ```
- **External Links (Diagonal Launch)**:
  ```html
  <a class="group inline-flex items-center gap-1.5">
    <span>Documentation</span>
    <IconExternal class="transition-transform duration-150 ease-out group-hover:translate-x-0.5 group-hover:-translate-y-0.5" />
  </a>
  ```
- **Disclosure Chevrons (Spring Rotation)**:
  ```html
  <IconChevron class="transition-transform duration-200 cubic-bezier(0.2, 0.9, 0.3, 1) group-aria-expanded:rotate-180" />
  ```

#### 4. Gliding Spring Indicator (Tabs and Segmented Controls)
Switching tabs, filters, or view modes must never be an instant 0ms color pop. The active background pill glides smoothly under the selected tab with spring momentum:
```html
<!-- Container with relative positioning -->
<div class="relative flex items-center rounded-xl bg-zinc-100 p-1 dark:bg-zinc-800">
  <!-- Active sliding pill (positioned via transform translate) -->
  <div 
    class="absolute top-1 bottom-1 rounded-lg bg-white shadow-xs transition-transform duration-200 cubic-bezier(0.18, 0.9, 0.28, 1) dark:bg-zinc-700"
    style="transform: translateX(var(--tab-offset)); width: var(--tab-width);"
  />
  <button class="relative z-10 px-3 py-1.5 text-xs font-semibold">Overview</button>
  <button class="relative z-10 px-3 py-1.5 text-xs font-semibold">Settings</button>
</div>
```

#### 5. Elastic Toggle and Switch Roll
Toggle switches should not snap with a lifeless linear slide. The switch thumb stretches slightly along its motion axis before settling with spring tension:
```css
.switch-thumb {
  transition: transform 0.2s cubic-bezier(0.18, 0.9, 0.28, 1), width 0.15s ease;
}
.switch-thumb:active {
  width: 22px; /* slight elastic stretch during thumb contact */
}
```

#### 6. Origin-Anchored Spatial Reveals (Menus, Popovers, Modals)
Menus, popovers, and dropdowns should feel anchored to the trigger that spawned them, expanding slightly from their anchor point:
```css
@keyframes popover-scale-in {
  from {
    opacity: 0;
    transform: scale(0.95) translateY(4px);
  }
  to {
    opacity: 1;
    transform: scale(1) translateY(0);
  }
}

.animate-popover-in {
  transform-origin: top left;
  animation: popover-scale-in 0.15s cubic-bezier(0.16, 1, 0.3, 1) forwards;
}
```

#### 7. Micro-Bounce Action Feedback (Completion Snaps)
When an action succeeds (copying text, bookmarking, marking complete, saving), reward the user with an organic overshoot bounce rather than a static text change:
```css
@keyframes micro-bounce {
  0% { transform: scale(0.85); }
  60% { transform: scale(1.14); }
  100% { transform: scale(1); }
}

.animate-micro-bounce {
  animation: micro-bounce 0.22s cubic-bezier(0.34, 1.56, 0.64, 1) forwards;
}
```

#### 8. Organic Luminance Sweep (Skeletons and Loading States)
Replace harsh flashing neon rings and dizzying spinners with a subtle, directional light sweep across neutral zinc surfaces:
```css
@keyframes shimmer-sweep {
  0% { transform: translateX(-100%); }
  100% { transform: translateX(100%); }
}

.skeleton-shimmer {
  position: relative;
  overflow: hidden;
  background-color: rgba(244, 244, 245, 0.8); /* zinc-100 */
}
.skeleton-shimmer::after {
  content: '';
  position: absolute;
  inset: 0;
  transform: translateX(-100%);
  background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.4), transparent);
  animation: shimmer-sweep 1.6s cubic-bezier(0.4, 0, 0.2, 1) infinite;
}
```

#### 9. Smooth Height and Disclosure Interpolation
Collapsible sections, FAQs, and detail disclosures should smoothly interpolate their height and opacity with organic deceleration rather than jump-cutting:
```css
.disclosure-content {
  display: grid;
  grid-template-rows: 0fr;
  transition: grid-template-rows 0.22s cubic-bezier(0.16, 1, 0.3, 1), opacity 0.2s ease;
  opacity: 0;
}
.disclosure-content.expanded {
  grid-template-rows: 1fr;
  opacity: 1;
}
.disclosure-inner {
  overflow: hidden;
}
```

#### Essential Easing Curves Reference
- **Organic Deceleration (Entrances, Reveals, Disclosures)**: `cubic-bezier(0.16, 1, 0.3, 1)` (180ms - 220ms)
- **Spring Elastic Release (Tabs, Sliders, Switches)**: `cubic-bezier(0.18, 0.9, 0.28, 1)` (200ms - 240ms)
- **Micro-Bounce / Overshoot (Feedback, Action Completion)**: `cubic-bezier(0.34, 1.56, 0.64, 1)` (200ms - 240ms)
- **Fast Switch Press (Active Clicks & Taps)**: `cubic-bezier(0.2, 0.9, 0.3, 1)` (100ms - 120ms)

---

## 6. Action Copy and Confirmation Modals

Buttons and dialogs must be concise, calm, and direct. Eliminate melodramatic AI warnings and redundant filler.

### Action Buttons

| AI Slop Copy | Human Friendly Action |
| :--- | :--- |
| Click here to finalize purchase | Place order |
| Proceed to remove item from cart | Remove |
| Confirm and persist user changes | Save |
| Terminate active session and logout | Log out |
| Dismiss this modal window | Close / Cancel |
| Initiate file download sequence | Download |

### Confirmation Dialogs
- **AI Slop**:
  ```
  Warning: Irreversible Data Modification Procedure
  Are you entirely sure you want to proceed with deleting this record? This action will permanently erase the entity from the remote database and cannot be recovered under any circumstances.
  [Cancel Operation] [Confirm Permanent Erasure]
  ```
- **Clean UI**:
  ```
  Delete project?
  This will permanently delete "Marketing Q4" and all associated files. This cannot be undone.
  [Cancel] [Delete project]
  ```

---

## 7. Empty States and Error Messages

Empty states and error messages should provide calm, actionable guidance instead of sounding like a server stack trace or a database query failure.

### Empty States
- **AI Slop**: `"Zero database records retrieved matching your filter criteria. Please formulate a new search query or click below to instantiate an entity."`
- **Clean UI**: `"No results found"` with subtext `"Try searching with a different term."`
- **AI Slop**: `"There are currently no active customer invoices stored in this workspace."`
- **Clean UI**: `"No invoices yet"` with a `"Create invoice"` button.

### Error Messages
- **AI Slop**: `"Fatal error 500: An unexpected internal server exception occurred in the upstream REST API gateway while processing payload."`
- **Clean UI**: `"Unable to load items. Check your internet connection and try again."`

---

## 8. The Universal 8-Point Anti-Slop Audit

Before shipping any UI component, PR, or template, run this 8-point check:

1. **The Affirmation Check**: Did you add any badges saying "Active", "Operational", or "Ready" just to show a feature works? Delete them.
2. **The Jargon Check**: Does the copy mention "inference", "telemetry", "payload", "pipeline", "ingestion", "database", or "cache"? Translate to everyday human words.
3. **The Subtitle Check**: Does any title have a descriptive paragraph under it that simply rephrases the title? Delete the subtitle.
4. **The Extension Dump Check**: Did you add a subhead listing file extensions like "PNG, JPG, WEBP, or GIF" under a simple upload button? Delete it. The label speaks for itself.
5. **The Neon Glow Check**: Are there any colored box-shadows, drop-shadow halos, or glowing hover outlines? Replace with neutral surface shifts.
6. **The Motion and Interaction Check**: Is the interaction a dead, generic CSS swap with 0ms cuts or flat linear transitions? Give it physical life: active press compression (`active:scale-[0.96]`), subtle card lift (`hover:-translate-y-0.5`), directional icon nudges, gliding tab indicators, or organic spring curves.
7. **The Verb Check**: Are button labels longer than two or three words without good reason? Trim to punchy, active verbs ("Save", "Delete", "Export").
8. **The Dialog Check**: Do confirmation modals read like legal disclaimers? Make them direct and plain ("Delete project? This cannot be undone.").
