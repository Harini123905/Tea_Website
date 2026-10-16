# NOTES.md: Mistvale Tea Co. assessment

Short notes on what I changed, what I could not know, and the questions I have for the team.
Items marked **[confirm]** need to be checked or completed by me before I submit.

---

## 1. Questions for the team (things I could not know)

1. **Free shipping threshold.** The original announcement bar said free shipping above ₹499, while the original code used ₹599. I did not know which is correct, so I used **₹599** as a temporary choice (the value is one variable, `FREE_SHIP_AT`, so it is a one-line change). Which amount is right?
2. **Footer copyright line.** It reads "© 2020 MistVale. All right reserved." BRAND.md says the company was founded in 2019, the brand is spelled "Mistvale", and "All right reserved" looks like a typo. The footer legal text is marked "do not edit", so **[confirm: I left it unchanged / I moved the copyright line out of the legal block and corrected it]**. Can you confirm the approved wording?
3. **Checkout.** The checkout form posts to `https://mistvale.example/cart/checkout`, which is not a real site. **[confirm which behaviour I kept:]**
   - *If I submit the form:* clicking Checkout fills the hidden form fields (`items`, `coupon`) and submits it. The browser will show an error page because the address does not exist in this demo. Is that the expected behaviour?
   - *If I show a notice only:* clicking Checkout shows one message ("Checkout is not connected in this demo store.") and does not submit the form. I chose this because the demo has no working backend. Should it submit the form instead?
4. **Delivery zones.** The delivery check uses the supplied `API` block, which covers only a few pincode prefixes. Any other valid pincode shows "Sorry, we do not deliver yet". The approved FAQ says delivery takes 2 to 5 working days depending on the pincode, but it does not say which areas are covered. Is the list complete?
5. **Coupon rules.** The code applies `WELCOME10` with a minimum subtotal of ₹399, a discount cap of ₹150, and gift boxes excluded. **[confirm: these match rules R1 to R8 in the task; list each rule number and how it is handled]**
6. **Rounding.** The cart total is rounded to a whole rupee, while the discount can have paise. Should totals show paise?

---

## 2. Claims removed because I could not verify them

- "Rated 4.9/5 by 10,000+ customers": removed. BRAND.md says only two products have real ratings, and no company-wide rating is given.
- "As seen on Shark Tank India": removed. It is not in the company facts, and BRAND.md says no fake awards or badges.
- **Diwali sale strip** ("SALE!!!" and the countdown): removed **[confirm]**. It was not in the required section list, it had a blinking animation, all caps and an exclamation mark, and the sale is not part of the company facts.
- The newsletter pop-up: replaced with an inline newsletter section, as the brand rules require.

I added no facts, ratings, reviews or awards of my own. Ratings appear only on the two products that have them (Darjeeling First Flush and Masala Chai Blend).

---

## 3. What I changed (summary)

- **Bugs:** cart quantity limit (maximum 5 per tea, and never more than stock), coupon rules, shipping bar and totals, filters, sort and search working together (with out-of-date search results ignored), pincode check, and a cart that is saved and cleaned when the page reloads.
- **Design:** colours as CSS variables, two font families in one Google Fonts link, an 8px spacing scale, one corner radius, button states (hover, focus, active, disabled), the required sections in order **[confirm: FAQ section added and the sale strip removed]**, and reduced-motion support.
- **Shopping experience:** quick view window for each tea, clear sold-out state, cart drawer with quantity buttons, toast messages, inline form errors, and a 2-column product grid on phones.
- **Technical:** viewport tag, meta description, canonical, Open Graph and Twitter tags, JSON-LD (Organization, Product, FAQPage), alt text, skip link, and a keyboard focus ring. **[confirm each of these is in the final file]**
- **Images:** product images (the 8th is the gift box), a hero banner and a logo made with an AI image tool. All prompts are in `PROMPTS.md`. **[confirm: all 8 product images exist]**

Not changed, as required: product `id`, `name` and `price`, the `API` block and the footer legal text.

---

## 4. Where AI got it wrong and what I fixed

- The first cart drawer did not open because the CSS for `.drawer.is-open` was missing. The script was running with no console error, so the problem was in the CSS. I added the rules and checked the drawer slides in.
- I tried variations with a glass of tea and with decorative figurines in place of the tea, but they did not match the brand rule "pack or tin plus a hint of the tea", so I did not use them. **[confirm: this is true, and say which final images I used]**
- **[add your own examples: a bug you caught, a suggestion you rejected, or a result you tested and found wrong]**

---

## 5. Known limitations

- The images are **[confirm: converted to WebP / still PNG]**, with sizes **[confirm: product images under 150 KB, hero under 250 KB]**.
- Only 6 AI product images were logged for the 8 teas **[confirm: all 8 product images are done]**.
- Tested at **[confirm: phone width 360px or 375px, and desktop]** in **[confirm: browser]**.
- The shop is a demo. Checkout, search and pincode check use the supplied simulated backend.
