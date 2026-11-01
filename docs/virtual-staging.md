# AI virtual staging

Virtual staging lets a user upload a room photo and get back a version with new furniture in a chosen style, so they can picture the space furnished.

## Decisions so far

- **Model:** Gemini 3.1 Flash Image API, called from a **Base44 backend function**. This replaced an earlier Cloudflare Workers AI plan.
- **First scope:** upload one furnished-room photo, choose room type and style, restyle the furniture. No accounts or payments in the test.
- **Speed is the top priority.** The target is about **5 seconds** per image so it feels instant, like Zillow's. A small cost ($10–20/month) is acceptable to get that speed.
- **Test** with around **100 users**, starting on a Base44 test site.
- **Longer term:** a hybrid approach. Use the paid API now and possibly self-host an open-source model on the VPS later.

## Offer idea

- **10 free virtual stagings per month for renters** who are searching for a place, funded by owner and agency subscriptions.

## Related

- There is a separate Base44 app, **"Virtual Staging AI"**, used for this work.
