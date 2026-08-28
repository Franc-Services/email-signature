FRANC — EMAIL SIGNATURE
=======================

Files
-----
signature.html        The signature. Open it in a browser to see it.
franc-bg.png          Card background (1040 x 596).
franc-logo-light.png  Wordmark, placed at 70 x 24.


STEP 1 — Host the two images
----------------------------
Email clients cannot load images from your computer. Upload
franc-bg.png and franc-logo-light.png somewhere public with an https
address (your website, e.g. https://www.franc.services/sig/franc-bg.png,
or any file host / CDN).

Then open signature.html in a text editor and replace three filenames
with those full https addresses:

  background="franc-bg.png"                    -> background="https://.../franc-bg.png"
  background-image:url('franc-bg.png')         -> url('https://.../franc-bg.png')
  <img src="franc-logo-light.png"              -> src="https://.../franc-logo-light.png"

Save. Reopen in a browser to confirm both still appear.


STEP 2 — Install it
-------------------
Gmail / Google Workspace
  Open signature.html in a browser. Select the whole card (click just
  above the top-left corner and drag past the bottom-right). Copy.
  Gmail > Settings > See all settings > General > Signature > Create
  new, then paste. Save changes at the bottom of the page.

Apple Mail (macOS)
  Mail > Settings > Signatures. Create a signature, then paste the
  copied card into it. Untick "Always match my default message font".

Outlook (web) and most other providers
  Same as Gmail: copy the rendered card from the browser and paste
  into the signature box.

Providers that accept raw HTML (Front, HubSpot, Missive, Superhuman)
  Paste the contents of signature.html between the COPY markers.


HOW IT BEHAVES
--------------
Gmail, Apple Mail, Outlook web, mobile   Full design, background image
                                         and all.
Outlook desktop (Windows)                Ignores background images and
                                         shows a solid #121210 card.
                                         All type stays white and
                                         legible.
Space Grotesk / Poppins                  Render where available. Gmail
                                         strips web fonts and falls
                                         back to Helvetica / Arial;
                                         sizes and layout are
                                         unaffected.

Card is 520px wide, which fits every desktop client and scales down on
mobile. Phone, email and website are live links.
