# Lumonere Studio Link Page

Mobile-first social media landing page for Lumonere Studio.

## Links
- Facebook: https://www.facebook.com/lumonerestudio
- Instagram: https://www.instagram.com/lumonerestudio
- TikTok: https://www.tiktok.com/@lumonerestudio26
- Email: lumonerestudio@gmail.com
- Phone: 0921 7171 451

## Contact behavior
- Email button: Gmail web on desktop; attempts Gmail app on phones, then falls back to the device mail app.
- Call button: opens the phone dialer using `tel:`.
- Text button: opens the SMS/texting app using `sms:`.

## GitHub Pages
1. Upload `index.html`, `style.css`, and the `assets` folder to the repository root.
2. Open **Settings → Pages**.
3. Use **Deploy from a branch**.
4. Select `main` and `/ (root)`.
5. Save.


## Customer photostrip access
- The homepage accepts the six-character code printed on a customer photostrip.
- Valid codes route to `photostrip.html?code=XXXXXX`, where the page looks up the image through the `get-photostrip` Supabase Edge Function.
- Keep all Supabase service-role keys, Google OAuth client secrets, and refresh tokens out of the public repository. The browser page should use only the Supabase publishable key.


## Public navigation additions
- `index.html`: Home, Past Events, and Our Services navigation links.
- `past-events.html`: portfolio landing page; actual event photos can be added once approved for public sharing.
- `services.html`: describes photobooth rental, print formats, custom layouts, and digital photostrip access.
- `style.css`: shared navigation and feature-page styles.

No Supabase Edge Functions, credentials, or gallery configuration were changed by this update. Review the homepage against your live version before publishing because the available local snapshot may not include every live-site edit.
