COVE LANDING PAGE: SETUP
========================

Upload everything in this folder, keeping the structure:
  index.html
  assets/   (logo, smiley, tagline, favicon, social share image)
  fonts/    (Fraunces 72pt SuperSoft, self-hosted)
  Courier Prime and Inter Tight load from Google Fonts.

BEFORE UPLOADING, open index.html in a text editor and replace:
  1. YOUR_POSTHOG_KEY          -> PostHog Project API key (starts phc_)
                                  If your PostHog project is US-hosted, change
                                  eu.i.posthog.com to us.i.posthog.com

POSTHOG EVENTS YOU'LL SEE
  $pageview / $pageleave         visits
  newsletter_form_focus          someone clicked into an email box
  newsletter_signup              form submitted
  instagram_click                Instagram link clicked
  Funnel suggestion: $pageview -> newsletter_form_focus -> newsletter_signup

GETTING IT LIVE ON GANDI
  A) If you have Gandi Web Hosting: upload the folder contents to the site's
     web root (htdocs) using SFTP or the file manager.
  B) If Gandi only holds the domain: deploy the folder free on Netlify
     (drag it onto app.netlify.com/drop) or Cloudflare Pages, add your custom
     domain there, then add the DNS records they give you under
     Gandi > Domain > DNS Records.

FONT LICENSING
  All fonts are free to use under the SIL Open Font Licence:
  Fraunces, Courier Prime and Inter Tight.
