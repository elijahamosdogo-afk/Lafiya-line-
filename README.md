# Lafiya Line dashboard

The GitHub Pages dashboard calls the Lafiya Line Express API at `https://lafiya-line-voice.onrender.com`. It uses live Supabase Auth for staff login and loads records only after the API confirms the signed-in staff profile and facility.

Live data stays in memory in the browser. The prototype seed data and simulator remain for local development only; live accounts do not use demo passwords or simulated call responses.

The Enrol page supports a new child or a vaccination record for a returning child, so multiple children remain linked to one caregiver and later doses stay on the same child record. Dose stage, age unit, language, consent, and facility are checked by the API and database.

Outbound calls are paused until the full approved recordings are available and Twilio is funded. The current repository contains four English/Hausa master recordings; Kanuri and the dose-specific next-dose closers are still missing. Do not enable calls from the Render environment until those assets are uploaded and the full audio flow is confirmed.
