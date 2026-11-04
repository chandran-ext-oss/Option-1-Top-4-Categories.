Isha Health Solutions — Option 1a landing page
==============================================

index.html      the complete page (HTML, CSS and JS in one file)
i/ , img/       photographs, the Isha mark, and the Figma step illustrations

HOW TO RUN
----------
The page loads its photographs over HTTP, and the 3D map and interior
views read them as WebGL textures. Opening index.html straight from the
file system will block those textures (browser CORS rule for file://),
so serve the folder instead:

    python3 -m http.server 8000

then open http://localhost:8000

Everything else — layout, type, motion — works from the file system.

WHAT LOADS FROM A CDN
---------------------
Motion One 10.18.0 ....... the animation engine (jsDelivr)
three.js r128 ............ the 3D campus map and interior views (cdnjs)
Instrument Serif, Hanken Grotesk ..... Google Fonts

All three are pinned to exact versions. With no network the page still
renders and reads correctly: motion is skipped, and the 3D views fall
back to the flat photographs.

NOTES FOR THE BUILD
-------------------
- Testimonials are sample copy and marked as such; they need real stories.
- Two blog titles are the Figma placeholders.
- The campus buildings on the map are indicative masses, not a survey.
- Interiors are flat photographs mapped onto a curved segment. Supply 360
  equirectangular shots and the same code renders them as true panoramas.
