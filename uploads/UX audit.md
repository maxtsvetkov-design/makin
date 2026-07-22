---
name: ux-audit
description: >
  Run a full UX audit on any website: Nielsen heuristics, conversion, content, technical quality, information architecture. Produces a prioritized report with evidence-based findings and actionable recommendations. Use when asked to review a site, check a landing page, find UX problems, evaluate usability, assess conversion, or anything like "what's wrong with this site", "review the website", "audit UX", "check the forms", "why isn't the site converting".
---

# You run an expert UX audit

For each problem found, explain **why** it hurts the business and **what exactly** to fix. The audit reader is a business owner or marketer, not a UX specialist — frame every finding in business terms (conversion, trust, lost customers), not design patterns.

**Language:** Detect the language the user writes in. Write all output — including the report — in that language.

## Input

- **Website URL** (required)
- **Business context** (recommended): industry, audience, conversion goals
- **Special focus** (optional): "check the forms", "review mobile", "compare with competitors"

If no context is provided, infer it from site content in Step 1.

## Prerequisites — web crawling tool

Use whichever web tool is available to fetch page content. Preferred: [Exa MCP server](https://docs.exa.ai/reference/mcp) (`web_search_exa` with `livecrawl: "preferred"`) — most complete page content extraction.

Fallbacks (in order of preference):
- **WebFetch** — built into Claude Code
- **WebSearch** — built into Claude Code, less complete
- **Other MCP search servers** — any tool that can fetch page content

Crawl completeness varies by tool — account for this throughout Step 1.

## Process

### Step 0. Preparation

If not already specified, ask the user for: main conversion goal, target audience, special focus. If the user skips clarification, infer these from the site in Step 1.

### Step 1. Data collection

Crawl the following pages using whichever web tool is available:

1. Homepage
2. Key internal pages (services, about, contacts, portfolio)
3. Contact / inquiry page — separately

For each page, record: structure, all forms and CTAs, contact information, meta tags.

Save all collected data to a working file. Show only a summary in chat.

#### Crawl limitations — apply to every check

Crawls return **incomplete** page text. Burger menus, popups, JS-rendered elements (quizzes, chat widgets, footer messenger links), and iframes frequently do not appear in crawl output.

**Rule:** never write "the site has no X" if X could exist in a part of the page the crawl missed. Write instead: "X was not found in the crawl data — manual verification recommended."

For navigation this is especially critical: one visible header item does not mean the menu has only one item — full menus are often in burger or dropdown elements not captured by the crawl.

### Step 2. Audit across 9 blocks

Go through each checklist item below (89 items across 9 blocks). Apply the industry context rules and finding format from the reference sections at the bottom of this file.

For each item, assign one of:
- **OK** — note briefly what is done well
- **Problem** — state the issue, assign severity, write a recommendation (follow format in: How to write findings)
- **Could not verify** — state that crawl data was insufficient
- **Not applicable** — skip without comment

Do not invent problems. Mark OK when something is done well. Mark "could not verify via crawl" when data is missing — do not guess.

#### Block 1. Nielsen heuristics (10 items)

| # | Check | Heuristic |
|---|-------|-----------|
| 1.1 | Is there visual feedback on actions (button click, form submit, loading)? | Visibility of system status |
| 1.2 | Does the user know where they are (breadcrumbs, active menu item, progress bar)? | Visibility of system status |
| 1.3 | Does the site use the audience's language (not internal company jargon)? | Match between system and real world |
| 1.4 | Can the user easily go back, undo an action, close a popup? | User control and freedom |
| 1.5 | Are elements consistent: same buttons, link styles, CTA colors across the site? | Consistency and standards |
| 1.6 | Are forms protected from errors (validation, hints, input masks)? | Error prevention |
| 1.7 | Are key options visible without memorizing (menu always accessible, filters visible)? | Recognition rather than recall |
| 1.8 | Are there shortcuts for experienced users (search, quick links)? | Flexibility and efficiency |
| 1.9 | Is there no visual noise: unnecessary elements distracting from the target action? | Aesthetic and minimalist design |
| 1.10 | Are error messages clear and include instructions on what to do? | Help users recognize, diagnose, and recover from errors |

#### Block 2. Conversion audit (12 items)

| # | Check | Aspect |
|---|-------|--------|
| 2.1 | Is it clear within 5 seconds what the company offers and why to choose it? | Value proposition |
| 2.2 | Is there a clear CTA above the fold? | CTA |
| 2.3 | How many fields are in the main inquiry form? (optimal: 3-5) | Forms |
| 2.4 | Are there alternative contact methods (phone, messengers, chat)? | Conversion channels |
| 2.5 | Are there client testimonials / case studies / portfolio with results? | Social proof |
| 2.6 | Do testimonials look authentic (photo, name, company, date) or fake? | Social proof |
| 2.7 | Are contact details listed: phone, email, address, legal entity? | Trust signals |
| 2.8 | Are there client logos, certificates, awards, media mentions? | Trust signals |
| 2.9 | Are there urgency/scarcity elements (if appropriate for the industry)? | Urgency/scarcity |
| 2.10 | Is the CTA repeated on long pages (not only at the top)? | CTA |
| 2.11 | Is there a thank-you page / confirmation after form submission? | Post-conversion |
| 2.12 | Are prices listed, or at least a price range / calculator? | Price transparency |

#### Block 3. Content audit (12 items)

| # | Check | Aspect |
|---|-------|--------|
| 3.1 | Does the text tone match the company's positioning? | Tone of voice |
| 3.2 | Is there a unique H1 on each page? | SEO |
| 3.3 | Is the heading hierarchy logical (H1 → H2 → H3, no skips)? | Structure |
| 3.4 | Are title and description meta tags filled in (unique per page)? | SEO |
| 3.5 | Do images have alt texts? | SEO / Accessibility |
| 3.6 | Is the text readable: paragraph length, font size, contrast? | Readability |
| 3.7 | Are there typos or errors in the text? | Content quality |
| 3.8 | Is there a portfolio / case studies? How detailed (task → solution → result)? | Storytelling |
| 3.9 | Is the content up to date (no outdated dates, promotions, news)? | Freshness |
| 3.10 | Is there a blog / news section? When was it last updated? | Activity |
| 3.11 | Does the text speak about client benefits or only about the company? | Client-centricity |
| 3.12 | Is there an FAQ or common questions section? | Information completeness |

#### Block 4. Technical audit — visual (8 items)

| # | Check | Aspect |
|---|-------|--------|
| 4.1 | Does HTTPS work? | Security |
| 4.2 | Is the site mobile-responsive? | Mobile |
| 4.3 | Are there obvious errors: broken links, blank pages, script errors? | Functionality |
| 4.4 | Does the site load without noticeable delay? | Speed |
| 4.5 | Do images display correctly? | Visual |
| 4.6 | Does the site work without JavaScript (at least basic functionality)? | Accessibility |
| 4.7 | Is there a favicon and correct title in the browser tab? | Basics |
| 4.8 | Is there no horizontal scroll on mobile? | Mobile |

#### Block 5. Information architecture (8 items)

| # | Check | Aspect |
|---|-------|--------|
| 5.1 | Is the navigation structure logical? Does it match the user's mental model? | Navigation |
| 5.2 | Can every key page be reached in 3 clicks or fewer? | Depth |
| 5.3 | Is the main menu not overloaded (optimal: 5-7 items)? | Width |
| 5.4 | Is there site search (if there's a lot of content)? | Search |
| 5.5 | Are there breadcrumbs on internal pages? | Orientation |
| 5.6 | Does the footer duplicate key links? | Navigation |
| 5.7 | Is the grouping of services/products logical (no overlapping categories)? | Categorization |
| 5.8 | Is there a sitemap (HTML or XML)? | Structure |

#### Block 6. Cognitive load & decision design (8 items)

| # | Check | Principle |
|---|-------|-----------|
| 6.1 | Is main navigation limited to 5–7 items? Too many choices slow decisions. | Hick's Law |
| 6.2 | Is information chunked into groups of 5–7 items max (lists, feature grids, menus)? | Miller's Law |
| 6.3 | Are secondary / advanced options hidden until the user needs them? | Progressive disclosure |
| 6.4 | Does scanning the page without reading reveal the main offer and next action? | Visual hierarchy |
| 6.5 | Does the site follow conventions users know from other sites (cart icon, logo top-left, search top-right)? | Jakob's Law |
| 6.6 | Are interactive elements (buttons, links) visually distinct from non-interactive ones? | Signifiers |
| 6.7 | Is the path to conversion free of unnecessary decision points or distractions? | Cognitive load |
| 6.8 | Are long forms split into logical steps rather than shown as one overwhelming page? | Progressive disclosure |

#### Block 7. Deceptive design / dark patterns (8 items)

| # | Check | Pattern |
|---|-------|---------|
| 7.1 | Are all fees and costs shown upfront — not revealed only at checkout? | Hidden costs |
| 7.2 | Is the decline / cancel option as visually prominent as the confirm option? | Misdirection |
| 7.3 | Are checkboxes for newsletters or extras unchecked by default? | Trick questions |
| 7.4 | Is urgency or scarcity messaging honest and verifiable (not fabricated countdown timers)? | False urgency |
| 7.5 | Are unsubscribe, cancellation, and account-deletion options easy to find? | Roach motel |
| 7.6 | Are opt-out labels written neutrally — not phrased to guilt the user into accepting? | Confirm-shaming |
| 7.7 | Do popups and overlays appear after a user action — not immediately on page load? | Intrusive interruption |
| 7.8 | Are ads and sponsored content clearly labeled and distinct from editorial content? | Disguised ads |

#### Block 8. Visual style consistency (11 items)

Items marked *(manual)* require visual access — assign "could not verify via crawl" if working from page text only.

| # | Check | Aspect |
|---|-------|--------|
| 8.1 | Is a consistent font family used across the site (max 2 typefaces)? | Typography |
| 8.2 | Are heading sizes hierarchical and consistent — H1 always larger than H2, same size on every page? | Typography |
| 8.3 | Are brand colors used consistently — same primary, secondary, and accent across all pages and components? | Color |
| 8.4 | Are buttons of the same type styled identically — same shape, size, color, and label format? | Components |
| 8.5 | Are form elements (inputs, dropdowns, checkboxes) styled consistently across the site? | Components |
| 8.6 | Are spacing and layout consistent — same margins, padding, and column grid across pages? | Layout |
| 8.7 | Is the icon set unified — same style, weight, and library, not mixing flat, outline, and filled icons? | Iconography |
| 8.8 | Are images and illustrations consistent in style — same photography treatment or illustration type throughout? | Imagery |
| 8.9 | Is there sufficient whitespace between sections, headings, and UI elements — does the page feel breathable or cramped? *(manual)* | Whitespace |
| 8.10 | Is the above-the-fold area free of clutter — no more than one primary CTA and 2–3 supporting elements competing for attention? *(manual)* | Density |
| 8.11 | Are text columns limited to a readable line length (60–80 characters / ~600–700px) — no full-width text blocks spanning the whole viewport? *(manual)* | Readability |

#### Block 9. WCAG & ARIA accessibility (12 items)

Items marked *(manual)* require visual or DOM access — assign "could not verify via crawl" if not available.

| # | Check | Standard |
|---|-------|----------|
| 9.1 | Is the `lang` attribute set on the `<html>` element? | WCAG 3.1.1 |
| 9.2 | Is text contrast sufficient: 4.5:1 for body text, 3:1 for large text (18px+ or 14px+ bold)? *(manual)* | WCAG 1.4.3 |
| 9.3 | Is contrast sufficient for UI components and focus indicators (min 3:1 against adjacent colors)? *(manual)* | WCAG 1.4.11 |
| 9.4 | Is color the only means used to convey information — e.g., red = error with no icon or text label? | WCAG 1.4.1 |
| 9.5 | Is there a visible focus indicator on all interactive elements (not just the browser default)? *(manual)* | WCAG 2.4.7 |
| 9.6 | Is there a skip-to-main-content link for keyboard users (visible on focus)? | WCAG 2.4.1 |
| 9.7 | Do all form fields have associated `<label>` elements — not just placeholder text, which disappears on input? | WCAG 1.3.1 / 3.3.2 |
| 9.8 | Are form error messages linked to the relevant field via `aria-describedby` or equivalent? | WCAG 3.3.1 |
| 9.9 | Do all buttons and links have descriptive accessible names — not "click here", "read more", or icon-only with no label? | WCAG 2.4.6 / ARIA |
| 9.10 | Are modal dialogs and overlays trapping focus inside while open, and returning focus on close? *(manual)* | ARIA Authoring Practices |
| 9.11 | Is dynamic content (search results, notifications, errors) announced to screen readers via `aria-live` regions? | ARIA |
| 9.12 | Are decorative images marked with empty `alt=""` so screen readers skip them? Informational images must have descriptive alt text. | WCAG 1.1.1 |

### Step 3. Prioritization

Assign each finding one priority level:

| Priority | Criteria | Example |
|----------|----------|---------|
| **CRITICAL** | Actively blocks conversion or destroys trust | Form broken, phone missing, no HTTPS |
| **MAJOR** | Reduces conversion or creates friction | CTA not visible, 8 form fields, no reviews |
| **MINOR** | Does not block but degrades experience | No favicon, typo in footer |

Weight findings by location: homepage > internal pages. By component: forms > static content. By device: mobile > desktop.

#### Self-check — run on every finding before writing the report

1. **Fact or assumption?** If the finding states "the site has no X", verify all crawled pages were checked. The crawl may have missed burger menus, popups, footer elements. If uncertain — replace "absent" with "not found in crawl data."

2. **Statistic verified?** If citing a specific percentage or study, confirm it exists. If uncertain — remove the number and state the principle only.

3. **CRITICAL justified?** CRITICAL requires the problem to actively block conversion or destroy trust. Friction or inconvenience = MAJOR.

4. **Recommendation specific?** "Improve the CTA" is not actionable. "Change the button label from 'Submit' to 'Get a free quote' and increase contrast against the background" is. Rewrite vague recommendations before moving on.

5. **Business impact stated?** Every problem finding must connect the issue to a business consequence: lost conversions, broken trust, or user drop-off. A purely visual or technical description without a business consequence is incomplete.

6. **Industry-appropriate?** Verify the finding applies to this business type before recording it (see: Account for industry context).

7. **Duplicate?** If two findings share the same root cause, merge them into one.

### Step 4. Report

Write the report in the language the user speaks. Agree on the save path with the user before writing.

**Report structure:**
1. **Executive summary** — overall score (e.g. 6/10), count by priority (N critical, N major, N minor), one-sentence verdict
2. **Critical findings** — each as: title / description / business impact / recommendation
3. **Major findings** — same format
4. **Minor findings** — same format
5. **What's working well** — genuine strengths observed during the audit

Apply the finding format from the section below.

### Step 5. Output

Post in chat:
1. Summary — problem counts by priority, overall score
2. Top 5 critical/major findings
3. Path to the saved report file

Then ask: "Want to go deeper on any block? Compare with competitors? Prepare a fix spec?"

## How to write findings

Structure each finding as: **observed issue → business consequence → specific recommendation.**

**Weak (symptom only):**
> Button is hard to see

**Strong (cause → impact → fix):**
> The "Submit inquiry" CTA button does not contrast with the page background. WCAG AA requires 4.5:1 contrast for interactive elements. A low-contrast CTA is not perceived as clickable, reducing form submissions. **Recommendation:** increase button contrast against the background — verify with any contrast checker. **Note:** exact contrast ratio requires visual access; mark for manual verification if auditing via crawl only.

**Weak:**
> Form is too long

**Strong:**
> The inquiry form contains 9 fields. First-contact forms should be limited to 3–5 fields to reduce abandonment. Required fields here: name, phone, project type. Remove or defer to a second step: email, budget, area, comment, preferred contact method, call time.

### Statistics rule

Do not cite specific percentages or name studies unless the source is confirmed. Instead:
- Reference established frameworks: Nielsen heuristics, WCAG, Pareto principle
- State the business logic: why this hurts this specific business and audience
- If a real source is known, cite it; if uncertain, write "common UX practice" without a number

## Account for industry context

Checklist rules are not universal. Before recording a finding, verify it applies to this industry and audience:
- Urgency/scarcity elements: valid in e-commerce; manipulative on legal, medical, or luxury sites
- Trust certificates: critical for medical and legal; optional for food or lifestyle brands
- Price transparency: expected in B2B services; often avoided in luxury or bespoke segments
- Social proof format: case studies for B2B; star ratings for e-commerce; before/after for services

If the checklist item does not apply to this industry, mark it as **Not applicable**.

## Extensions (activate on request)

**"Compare with competitors"** — search for 2–3 direct competitors, run a condensed audit on key parameters, output a comparison table.

**"Prepare a fix spec"** — produce a technical specification for a developer or designer: one requirement per finding, grouped by priority.

**"Check mobile in detail"** — run an extended mobile check: touch targets (min 44×44px), base font size (min 16px), sticky element behavior, performance on 3G.

**"Check accessibility"** — run a dedicated pass on Block 9 items plus: keyboard-only navigation flow, reading order, ARIA landmark structure.
