Isha Health Solutions - homepage (static site)

Contents
  index.html   the full page (HTML, CSS and JS in one file)
  img/         all photographs and illustrations used

Deploy (any static host, no build step)
  Netlify : drag this folder onto app.netlify.com/drop
  Vercel  : run `vercel --prod` inside this folder
  S3 / CDN / Nginx / Apache : upload index.html and img/ to the web root

Needs internet access for two external resources:
  Google Fonts (Plus Jakarta Sans) and the Motion One script from cdn.jsdelivr.net.
  If your site uses a strict Content-Security-Policy, allow fonts.googleapis.com,
  fonts.gstatic.com and cdn.jsdelivr.net.

Before launch
  - Replace the sample patient stories, doctor names and qualifications with verified content.
  - Replace the sample article list with real articles and link the "Explore program" cards to program pages.
  - Add the virtual tour video and wire the play button; add contact details in the footer.
  - Connect the call-back form (it currently only shows a thank-you message; nothing is sent).
  - Replace stock photography where licences are not confirmed.
