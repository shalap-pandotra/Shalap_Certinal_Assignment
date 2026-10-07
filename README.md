# Quoted

**Know what to charge brands.** An AI price check, counter-offer drafter and deal board for micro-creators in India. Built for a take-home assignment: design an AI-powered product that helps influencers grow and monetize.

## Start here

| | Link | What it is |
| --- | --- | --- |
| **Live Site (access given to panelists)** | [Open the live prototype](https://claude.ai/artifact/AWYuRhqaz76TNPwfnedU9X) | The full prototype with live AI. Invite-only: see the sign-in steps below. |
| **Demo (no sign-in)** | [Open the demo](https://shalap-pandotra.github.io/) | The same screens with pre-written examples instead of live AI. Open to anyone. |
| Product spec | [PDF](Quoted_product_spec.pdf) | Problem, personas, product, value, go-to-market, assumptions and risks. |
| Journeys and wireframes | [PDF](Quoted_journeys_and_wireframes.pdf) | Two journey maps and the wireframes. |
| Part B: the AI | [Markdown](prompts_evals_guardrails.md) | Both prompts, 10 evals and 5 guardrails. |

## Signing in to the Live Site

The Live Site is a Claude artifact, so it opens inside Claude.

1. Open the link. If you are signed out, sign in to Claude with the email address the panel was invited on.
2. Choose **Open artifact**.
3. Go to **Price a deal**, load an example and press **Price this deal**. The first time, allow the permission prompt.

The AI runs on your own Claude account, so each price check or drafted reply uses a little of your Claude usage. If you cannot sign in, use the Demo instead.

## Demo or Live Site

| | Demo | Live Site |
| --- | --- | --- |
| Home, Price a deal and Deals screens | Yes | Yes |
| The four example inputs | Pre-written results | Priced live by Claude |
| Your own numbers | Not priced | Priced live by Claude |
| Draft reply to brand | No | Yes |
| Needs a Claude sign-in | No | Yes |

## What to try

- **Example: 80k followers, 0.2% engagement.** A large following with thin reach. The price should follow reach, not followers.
- **Example: reel plus YouTube Short.** A two-platform package, each priced from its own numbers.
- **Example: stats missing.** The page refuses to name a price and says exactly what it needs.
- **Live Site only:** type your own numbers, then press **Draft reply to brand** and save the deal. Part B lists ten inputs worth running, including ones built to break it.

## The idea in brief

- **Problem:** small creators quote by gut feel or follower count, while brands and agencies increasingly price with deal data.
- **Product:** a price check built on reach that shows its math and says when it is unsure, a counter-offer draft, and a board that tracks every deal.
- **Value metric:** money left on the table, the gap between what a creator accepts and the bottom of a fair range.

## How it is built

- One HTML file, no backend. The AI call uses the Claude artifact runtime, which is why the Live Site needs a Claude sign-in.
- The guardrails sit in code as well as in the prompt: missing-stats and implausible-view checks, the offer-versus-range verdict, and a paid-partnership reminder on every result.
- All creators, brands and prices in the prototype are made up. Figures in the spec marked "assumed" are mine, not sourced.
