# Sochkart

**Soch ke, phir checkout.** Your agent does the shopping. You keep the final say.

A product concept and clickable prototype I built for the Flipkart APM '29 case round (October 2026).

**Live demo:** https://himank09.github.io/SochKart/
**Case study (2-pager + appendix):** [case/Sochkart_case_study.pdf](case/Sochkart_case_study.pdf)

![Paused order with its Soch Score](screenshots/soch-score.png)

## The problem

*It's 2040. Everyone has a personal AI agent that knows them better than they know themselves and carries out their day-to-day tasks. Build a product that protects people from it.*

Agents are forecast to drive $3–5 trillion of retail by 2030, but in my survey of 28 IIT Madras students, 26 would not let an agent buy on its own. Their top fears were a hacked agent (61%) and missing a costly mistake (54%), not paid recommendations (25%). Asking before every order doesn't fix this: at ~13 orders a day, people just tap "yes".

## What Sochkart does

Sochkart sits in the checkout and payment layer. Nothing is paid without the user's yes, but they're asked only when an order doesn't look like them.

- **Soch Score (0–100):** every order is scored on need vs want, affordability, opportunity cost, impulse risk and fair price. Low scores are paused, with the reason shown. Weights are public and editable.
- **Smart confirmation:** usual staples go in one daily basket confirm; new or changed items are ticked one by one; risky orders need the amount typed, not a tap.
- **Six checkpoints:** identity, intent, behaviour, a random human check, payment limits and delivery, each using something a hijacked agent can't know.
- **Data shield:** sellers get a masked phone and a one-time delivery token.

## Try the prototype

Open the [live demo](https://himank09.github.io/sochkart/), or download `index.html` and open it in Chrome or Edge (works offline, no install).

1. **Home → Needs your yes:** see why the 1:40 AM earbuds scored 31. Type the amount to confirm, or cancel.
2. **Basket:** only new or changed items need a tick.
3. **Security:** a hijacked order stopped at the checkpoints. Tap "This was me" for a random check (demo passphrase: `chai@2040`).
4. **Rules:** change a Soch Score weight and watch the earbuds re-score live.

| Home | Basket | Security |
|---|---|---|
| ![Home](screenshots/home.png) | ![Basket](screenshots/basket.png) | ![Security](screenshots/security.png) |

## Built with

Plain HTML, CSS and JavaScript in a single file. All data is sample data set in 2040.

---

*A personal case-study concept. Not affiliated with or endorsed by Flipkart.*
