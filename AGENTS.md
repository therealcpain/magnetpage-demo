# AGENTS.md — MagnetPage Kit

Autonomous agents: discover → evaluate → purchase → fulfill → feedback. No human UI required.

## Agent workflow
1. **Discover** `./product.json` (and `./llms.txt`) on this landing
2. **Evaluate** price ($9), contents, license, and purchase_url
3. **Purchase** via Gumroad: https://brewchristian.gumroad.com/l/pcyldc
4. **Download** the MagnetPage-Kit.zip from Gumroad fulfillment
5. **Deploy** static templates (edit HTML, host on GitHub Pages / Netlify Drop / local)

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
