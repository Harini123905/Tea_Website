PROMPTS.md: Mistvale Tea Co. assessment

Prompts are copied exactly as typed, including typos.

Part 1: Claude (claude.ai chat), used for understanding the task and for code.
Part 2: Image generation, used for the 8 product images, the gift box, the hero banner and the logo. Tool used: [write the name of the image tool].
Part 1: Chat and code prompts
Prompt 1

Prompt: this is my task can you explain this (followed by the pasted assessment text, "Developer Assessment: Rescue the Mistvale tea store")

AI output: Plain-language summary: the five jobs, the rules (one index.html, no libraries, don't change id/name/price, API block or footer legal text), and the hand-in files. What I checked / changed: [write what you did, e.g. re-read the original task to confirm the rules]

Prompt 2

Prompt: [pasted the full index.html] [add any words you typed with it]

AI output: Explanation of the file's three parts. Flagged suspicious items: unverifiable claims ("Rated 4.9/5 by 10,000+ customers", "As seen on Shark Tank India") and a shipping threshold conflict (₹499 in the banner vs ₹599 in the code). What I checked / changed: [e.g. checked these against BRAND.md]

Prompts 3 to N (MISSING: copy from your chat)

These came between the index.html paste and the console message. They cover:

pasting BRAND.md
design and bug-fix requests (cart, quick view, filters, coupon)
the message where the cart button stopped working after a large paste
any screenshots sent (write "screenshot of ..." and what it showed)

Use this block once for each message:

Prompt: [exact text] AI output: [one line] What I checked / changed: [one line]

Prompt: console check

Prompt: in console bar not showing error

AI output: Diagnosis that the script was running and the problem was missing CSS (.drawer.is-open). Gave the cart drawer, cart line, totals and toast CSS to paste before </style>. What I checked / changed: [e.g. searched for .drawer.is-open, added the CSS, confirmed whether the drawer slides in]

Prompt: checkout notification

Prompt: now i want if i click checkout just it will show one notify give this code

AI output: A script that shows one toast when Checkout is clicked. The button selector was a guess (#checkout-btn, #checkout, .checkout-btn). The AI also warned that replacing the required checkout form could lose marks. What I checked / changed: [e.g. replaced the guessed selector with my real one; decided to keep only the notification; added a note to NOTES.md]

Prompt: first log request

Prompt: ok give me prompt log for this prpoject

AI output: A PROMPTS.md template with gaps marked for the prompts it could not see. What I checked / changed: [e.g. noticed it was incomplete and asked for the full version]

Prompt: full log request

Prompt: i want total prompt logs

AI output: A fuller version of this log. What I checked / changed: [e.g. filled in the missing prompts from my chat history]

Prompt: add image prompts

Prompt: can you this prompt also in this log file

AI output: This file, with Part 2 (image prompts) added. What I checked / changed: [e.g. checked every prompt is copied exactly as typed]

Part 2: Image generation prompts

Note: for the prompts marked "(reference image attached)", I uploaded a reference image with the message.

Image Prompt 1: Dark Green Tea Tin

Prompt: Square 1:1 product photograph of a matte dark green tea tin with a plain unlabelled front, standing on a pale linen cloth. A small wooden spoon of dark, malty CTC black tea leaves rests beside the tin. Soft natural window light from the left, gentle soft shadows, calm cream and warm wood tones, shallow depth of field, premium and calm mood. No text, no logos, no labels, no people generate this image

AI output: Generated a premium square tea product photograph featuring a matte dark green tea tin and loose CTC black tea. What I checked / changed: Checked the tin color, tea leaves, lighting and unlabelled design.

Image Prompt 2: Glass Instead of Tea

Prompt: i want this box instead of tea there in glass

AI output: Generated the tea tin with a glass of brewed tea beside it. What I checked / changed: Checked that the glass replaced the tea presentation.

Image Prompt 3: Reference Image

Prompt: i want likw this just take reference (reference image attached)

AI output: Used the supplied reference image to create a similar warm, cinematic tea composition. What I checked / changed: Checked the composition, lighting and placement against the reference.

Image Prompt 4: Sage Green Tea

Prompt: Square 1:1 product photograph of a matte sage green tea tin with a plain unlabelled front, standing on a pale linen cloth. A small wooden spoon of delicate, twisted whole tea leaves in pale green and golden tones rests beside the tin. Soft natural window light from the left, gentle soft shadows, calm cream and warm wood tones, shallow depth of field, premium and calm mood. No text, no logos, no labels, no people.

AI output: Generated a sage-green tea product photograph with loose green tea leaves. What I checked / changed: Checked the sage-green tin and natural premium styling.

Image Prompt 5: Glass of Tea

Prompt: in this container box instead of u can add glass of tea

AI output: Generated the sage-green tea setup with a glass of brewed tea. What I checked / changed: Checked that the glass was used instead of the container arrangement.

Image Prompt 6: Reference Again

Prompt: actually i gave one reference image you can take this (reference image attached)

AI output: Used the supplied reference image to create a closer matching tea composition. What I checked / changed: Compared the generated image with the reference.

Image Prompt 7: Fresh Leaf Green Tea

Prompt: Square 1:1 product photograph of a matte fresh leaf green tea tin with a plain unlabelled front, standing on a pale linen cloth. A small wooden spoon of smooth, rolled green tea leaves rests beside the tin. Soft natural window light from the left, gentle soft shadows, calm cream and warm wood tones, shallow depth of field, premium and calm mood. No text, no logos, no labels, no people. take this image reference (reference image attached)

AI output: Generated a fresh green tea product scene based on the supplied reference. What I checked / changed: Checked the green tea leaves, tin color and reference composition.

Image Prompt 8: Toys / Couple Statue

Prompt: in this container box instead of you can any toys or couple statue

AI output: Generated the tea scene with decorative couple/teddy-bear figurines replacing the container. What I checked / changed: Checked whether the decorative elements fit naturally into the tea scene.

Image Prompt 9: Chamomile + Tulsi

Prompt: Square 1:1 product photograph of a matte soft cream and ochre tea tin with a plain unlabelled front, standing on a pale linen cloth. A small wooden spoon of dried chamomile flowers and dried green holy basil leaves rests beside the tin. Soft natural window light from the left, gentle soft shadows, calm cream and warm wood tones, shallow depth of field, premium and calm mood. No text, no logos, no labels, no people. take tis image reference (reference image attached)

AI output: Generated a cream-and-ochre herbal tea scene featuring Chamomile and Tulsi. What I checked / changed: Checked that both chamomile flowers and tulsi leaves were represented.

Image Prompt 10: Hibiscus + Rose

Prompt: Square 1:1 product photograph of a matte dusty rose tea tin with a plain unlabelled front, standing on a pale linen cloth. A small wooden spoon of dried deep red hibiscus petals and dried pink rose petals rests beside the tin. Soft natural window light from the left, gentle soft shadows, calm cream and warm wood tones, shallow depth of field, premium and calm mood. No text, no logos, no labels, no people. take this reference i want this image exactly (reference image attached)

AI output: Generated a dusty-rose tea product scene featuring hibiscus and rose petals. What I checked / changed: Checked the dusty-rose color and hibiscus/rose ingredients.

Image Prompt 11: Six-Tin Gift Box

Prompt: Square 1:1 product photograph of an open wooden gift box standing on a pale linen cloth, holding six small matte tea tins in muted green, olive, terracotta, cream and rose tones, with a plain folded cream card tucked beside them. A few loose tea leaves are scattered on the linen. Soft natural window light from the left, gentle soft shadows, calm cream and warm wood tones, shallow depth of field, premium and calm mood. No text, no writing on the card, no logos, no labels, no people. reference image (reference image attached)

AI output: Generated an open wooden tea gift box containing six muted-color tea tins and a blank cream card. What I checked / changed: Checked the six tins, colors, wooden box and blank card.

Image Prompt 12: Wide Hero Image

Prompt: Wide 3:2 landscape photograph of a calm wooden table by a window in soft morning light. On the table are a ceramic cup of freshly brewed tea with gentle steam, a small teapot, and a few matte tea tins in muted green, terracotta and cream tones, with a handful of loose tea leaves on pale linen. Out-of-focus green hills softly visible through the window behind. Soft natural light, gentle soft shadows, calm cream, warm wood and soft green tones, shallow depth of field, premium and peaceful mood. Leave some calm empty space. No text, no logos, no labels, no people.

AI output: Generated a wide landscape tea-table image suitable for the website hero section. What I checked / changed: Checked the empty space for website text and the calm premium atmosphere.

Image Prompt 13: Mistvale Logo

Prompt: Simple flat vector logo for a tea brand. A small minimal leaf mark in cream beside the word "Mistvale" in an elegant serif font, all on a solid dark forest green background. Only two colours: cream and dark green. Clean sharp edges, no gradients, no shadows, no texture, no extra text, no tagline, no border. Wide horizontal layout with the leaf on the left and the word on the right. Calm, premium and simple.

AI output: Generated a horizontal Mistvale logo with a cream leaf mark and serif wordmark on a dark forest-green background. What I checked / changed: Checked the two-color restriction, horizontal layout, leaf placement and absence of extra text.