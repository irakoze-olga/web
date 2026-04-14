<div align="center">

<svg width="520" height="70" viewBox="0 0 520 70" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="orangeGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#ff6b2b" stop-opacity="0"/>
      <stop offset="40%" stop-color="#ff9f1c" stop-opacity="1"/>
      <stop offset="60%" stop-color="#ff6b2b" stop-opacity="1"/>
      <stop offset="100%" stop-color="#ff6b2b" stop-opacity="0"/>
    </linearGradient>
  </defs>

  <!-- Background bar -->
  <rect x="60" y="33" width="400" height="3" rx="2" fill="url(#orangeGrad)" opacity="0.25"/>

  <!-- Animated progress fill -->
  <rect x="60" y="33" width="0" height="3" rx="2" fill="url(#orangeGrad)">
    <animate attributeName="width" values="0;400;0" dur="2.8s" repeatCount="indefinite" calcMode="spline" keySplines="0.4 0 0.2 1;0.4 0 0.2 1"/>
  </rect>

  <!-- Delivery scooter dot riding the bar -->
  <circle r="6" fill="#ff6b2b">
    <animate attributeName="cx" values="60;460;60" dur="2.8s" repeatCount="indefinite" calcMode="spline" keySplines="0.4 0 0.2 1;0.4 0 0.2 1"/>
    <animate attributeName="cy" values="35;35;35" dur="2.8s" repeatCount="indefinite"/>
  </circle>

  <!-- Start pin -->
  <circle cx="60" cy="35" r="3" fill="#ff9f1c" opacity="0.6"/>
  <!-- End pin -->
  <circle cx="460" cy="35" r="3" fill="#ff9f1c" opacity="0.6">
    <animate attributeName="opacity" values="0.2;0.9;0.2" dur="2.8s" repeatCount="indefinite"/>
  </circle>

  <!-- Label -->
  <text x="260" y="58" text-anchor="middle" font-family="monospace" font-size="9" fill="#ff9f1c" opacity="0.7" letter-spacing="4">DELIVERING NEAR YOU</text>
</svg>

# Quick Food

**Hot meals. Fast delivery. Zero hassle.**

</div>

---

## What This Document Covers

This file is the full content and design reference for the **Quick Food** food delivery website. It is written for developers, designers, and contributors to understand every section of the site — what goes in it, how it should look, and how it should behave.

---

## Site Structure

Quick Food is a single-page website with six clearly defined sections:

| Section | Purpose |
|---|---|
| Hero | Grab attention, show the value proposition, prompt first order |
| How It Works | Explain the delivery process in three simple steps |
| Menu Categories | Show what kinds of food are available |
| Featured Dishes | Highlight popular or promoted items |
| Delivery Info | Coverage area, fees, and estimated times |
| Footer | Links, app download prompts, and legal copy |

---

## Section 1 — Hero

The hero is the highest-stakes part of the page. A visitor decides within seconds whether to stay or leave. The message must be immediate and the action obvious.

**Content to include:**

- A bold headline that communicates speed and appetite:
  > *Your favourite food, at your door in 30 minutes.*
- A short supporting line beneath it:
  > *Order from the best local restaurants. Track your delivery live.*
- A postcode or address input field with a prominent button labelled `Find Food Near Me`
- A small trust line beneath the input, for example: *Free delivery on your first order.*
- A looping, muted background visual suggesting warmth and motion (a blurred kitchen scene or abstract food photography works well)

**Design notes:**

Use a warm, high-energy palette. Orange is the primary action colour. The headline should be large and bold — this is not the place for refinement. The input and button should sit on the same line on desktop and stack on mobile.

---

## Section 2 — How It Works

This section removes friction. First-time visitors need to feel that ordering is easy before they commit.

**Display three steps in a horizontal row:**

**Step 1 — Choose Your Food**
Browse restaurants and dishes near your location. Filter by cuisine, rating, delivery time, or price.

**Step 2 — Place Your Order**
Add items to your basket, review your order, and pay securely in under a minute.

**Step 3 — Track Live**
Watch your order move from the kitchen to your door in real time on a live map.

**Design notes:**

Number each step clearly (`01`, `02`, `03`). Connect them with a dashed or dotted line to suggest progression. Keep the descriptions short — two sentences maximum per step. On mobile, stack vertically and hide the connecting line.

---

## Section 3 — Menu Categories

Visitors arrive with a craving. This section helps them find it fast. Show categories as tappable cards in a horizontal scroll on mobile and a grid on desktop.

**Categories to include:**

| Category | Description |
|---|---|
| Burgers | Classic, smash, gourmet, plant-based |
| Pizza | Thin crust, deep dish, loaded, vegan |
| Sushi | Rolls, nigiri, sashimi, bento boxes |
| Chicken | Fried, grilled, wraps, wings |
| Pasta | Carbonara, bolognese, baked, creamy |
| Salads | Fresh, grain bowls, protein-loaded |
| Desserts | Cakes, ice cream, waffles, brownies |
| Drinks | Juices, milkshakes, sodas, smoothies |

**Design notes:**

Each card should show the category name and a single illustrative image. Hovering a card on desktop should lift it slightly with a shadow. Tapping on mobile should navigate to a filtered restaurant list. Avoid cluttering the cards with prices or ratings — keep them clean and inviting.

---

## Section 4 — Featured Dishes

Highlight three to four dishes that are either popular, promoted by a partner restaurant, or seasonal. This section drives impulse decisions.

**Each dish card should include:**

- Dish name
- Restaurant name and rating
- Short description (one line)
- Price
- Estimated delivery time
- An `Add to Basket` button

**Example entries:**

| Dish | Restaurant | Price | Time |
|---|---|---|---|
| Double Smash Burger | The Grill House | 12.50 | 25 min |
| Truffle Margherita | Napoli Express | 14.00 | 20 min |
| Spicy Tuna Roll (8 pcs) | Sakura Kitchen | 13.00 | 30 min |
| Crispy Chicken Wrap | Street Bird | 9.50 | 18 min |

**Design notes:**

Cards should be horizontal on desktop (image on the left, details on the right) and vertical on mobile. The delivery time and price should be visually prominent. The `Add to Basket` button uses the primary orange colour.

---

## Section 5 — Delivery Info

Transparency builds trust. This section tells the customer exactly what to expect before they order.

**Content to include:**

**Coverage**
Quick Food currently delivers across the following areas. Entering a postcode on the hero section confirms availability instantly.

- City centre and inner districts: full coverage
- Suburbs within 8 km: full coverage
- Outer areas beyond 8 km: partner-dependent, shown at checkout

**Delivery Fees**

| Order Value | Delivery Fee |
|---|---|
| Under 15.00 | 2.99 |
| 15.00 to 30.00 | 1.49 |
| Over 30.00 | Free |

> First-time customers always receive free delivery regardless of order value.

**Estimated Times**

Delivery times depend on restaurant preparation time and distance. The average across all orders is 28 minutes. Live tracking is available from the moment an order is confirmed.

**Design notes:**

Use a clean two-column layout — coverage and times on the left, fees on the right. A small inline map showing the delivery radius adds credibility. Keep the tone factual and reassuring, not salesy.

---

## Section 6 — Footer

The footer closes the page and provides utility links, app download prompts, and legal copy.

**Content to include:**

- Quick Food logo and tagline: *Hot food, fast.*
- App download buttons for iOS and Android
- Four columns of links:

| Column | Links |
|---|---|
| Company | About Us, Careers, Press, Blog |
| Help | FAQ, Contact Support, Track Order, Report an Issue |
| Partners | List Your Restaurant, Become a Driver, Partner Portal |
| Legal | Privacy Policy, Terms of Service, Cookie Settings |

- Social media links: Instagram, TikTok, X (Twitter)
- Copyright line: `Quick Food — All rights reserved`

---

## Typography

| Role | Font | Weight | Notes |
|---|---|---|---|
| Headings | Poppins | 700–800 | Rounded, friendly, high energy |
| Body | Poppins | 400 | Same family keeps it cohesive |
| Labels / Tags | Poppins | 500–600 | Uppercase for category labels |
| Prices / Times | Poppins | 600 | Slightly larger than body |

Poppins is available on Google Fonts. Load only the weights actually used to keep page load fast.

---

## Color Palette

| Name | Hex | Usage |
|---|---|---|
| Orange | `#ff6b2b` | Primary buttons, highlights, icons |
| Amber | `#ff9f1c` | Hover states, secondary accents |
| White | `#ffffff` | Backgrounds, card surfaces |
| Off-white | `#faf8f5` | Alternate section backgrounds |
| Dark | `#1c1a18` | Primary text, footer background |
| Grey | `#6b6560` | Secondary text, descriptions |
| Light Grey | `#e8e4df` | Borders, dividers |

---

## Animations

Animations should feel quick and functional — they should reinforce the brand idea of speed, not slow the experience down.

- **Top delivery bar** — an orange dot travels from left to right across a progress bar on page load, suggesting a live delivery in motion
- **Hero entrance** — headline fades in and rises slightly over 0.5 seconds; the input field follows 0.2 seconds later
- **Category card hover** — card lifts 4px with a soft shadow on hover; transition duration 0.2s
- **Dish card add button** — button pulses briefly when clicked to confirm the item was added to the basket
- **Step connector** — the dashed line between the three How It Works steps draws in left to right on first scroll into view

All animations should respect the `prefers-reduced-motion` media query. If a user has this setting enabled, all transitions should be instant.

---

## Responsive Behaviour

| Breakpoint | Changes |
|---|---|
| Below 480px | Single column throughout; hero input and button stack; category row becomes horizontal scroll |
| 480px to 768px | Two-column category grid; dish cards go vertical |
| Above 768px | Full layout as described in each section above |

---

## Performance Notes

Food delivery sites lose conversions fast if pages are slow. Keep the following in mind:

- Compress all food images to WebP format at 80% quality
- Lazy-load images below the fold
- Load Google Fonts with `display=swap` to avoid invisible text on slow connections
- Target a Largest Contentful Paint of under 2.5 seconds on a mid-range mobile device

---

*This document is a living reference. Update it whenever the menu categories, delivery zones, pricing, or design direction changes.*