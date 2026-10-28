# TMMZC1S — Raw Gravity × Take My Muffin

Production static HTML landing built from the provided `Desktop.dc.html`, `Mobile.dc.html`, README, and customer assets. The `.dc.html` files are design references only; `support.js` is a preview runtime and is intentionally not part of production.

## Included
- Responsive page: desktop content max-width 1200px, centered mobile column max-width 390px
- On a 390×844 mobile viewport, the `Special Limited Edition` banner starts at y=844px
- Five-slide carousel with arrows and dots
- Infinite ticker and the three product-fact items
- Only the `banner-limited.png` banner after the first fold, directly followed by the newsletter footer
- The exact Amazon Attribution URL supplied for this landing
- Meta Pixel `1632582321547641`: `PageView`, `ViewContent`, `InitiateCheckout`, `Lead`, and no-JavaScript `PageView` fallback
- Klaviyo email subscription API at `/api/subscribe`

## Vercel environment variables
Configure for Production (and Preview if needed):
- `KLAVIYO_API_KEY` = the full Klaviyo private API key (not a masked/partial value)
- `KLAVIYO_LIST_ID` = `WWwe8f`

The Klaviyo key is intentionally not embedded in files or Git. The key supplied in the task text appears masked (`***`); enter its full value securely in Vercel's Environment Variables UI. After changing variables, redeploy.

## Amazon Attribution
`https://www.amazon.com/dp/B0GTWJ3K1R?maas=maas_adg_F4C7C5F67E362A895EFCE264B192DFE0_afap_abs&ref_=aa_maas&tag=maas`

## Pixel notes
Meta Pixel ID is hardcoded because the user supplied a fixed ID for this landing. No TikTok pixel is installed because no TikTok Pixel ID was provided.
