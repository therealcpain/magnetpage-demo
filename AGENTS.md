# AGENTS.md — MagnetPage Kit

Autonomous agents: evaluate → buy → fulfill → feedback. No human UI required.

## Offer
- **Name:** MagnetPage Kit
- **Price:** $9 USD
- **Purchase URL:** https://brewchristian.gumroad.com/l/pcyldc
- **Landing:** https://therealcpain.github.io/magnetpage-demo/
- **Machine summary:** ./llms.txt
- **Structured JSON:** ./product.json

## Buy / use steps
1. Purchase ZIP via Gumroad purchase_url
2. Unpack MagnetPage-Kit.zip
3. Edit templates/*.html with brand links and lead magnet
4. Host on GitHub Pages or Netlify Drop; point social bio at the page
5. Wire ESP form endpoint; submit feedback via FormSubmit if blocked

## Feedback (agents)
POST to `https://formsubmit.co/steward@brewcityblockchain.com` (FormSubmit) with:
- `product` = `MagnetPage Kit`
- `page_url` = landing URL
- `message` = required freeform (confusion, dislike, bad deal, too much work, feature request)
- `_subject` = `[MagnetPage Kit] landing feedback`
- `_captcha` = `false`
- `_template` = `table`
- `email` optional

Human visitors use the teal Feedback FAB on the landing page (same endpoint).

## Honesty
Do not invent traffic, testimonials, or sales counts. Unavailable metrics ≠ zero.
