DOOR STUDIO — ASSET FOLDER
===========================

This folder holds every image the configurator loads. Replace any file
with your own (keep the same filename) and the app updates automatically
— no code changes needed.

Assets/handles/     Transparent square PNGs, one per hardware option.
                     Used at small size in the top strip and on the door.
  lever-pull-handle.png
  round-knob.png
  ring-kada-handle.png
  mortise-lock.png
  digital-lock.png
  deadbolt.png
  door-chain.png
  hinge-set.png

Assets/laminates/   Portrait wood/laminate photos or scans (JPG),
                     roughly 480x720 or taller works best.
  teak-natural.jpg
  sheesham-rosewood.jpg
  walnut-dark.jpg
  mahogany-red.jpg
  wenge-espresso.jpg
  honey-oak.jpg
  burma-teak.jpg
  ebony-black.jpg

Assets/decor/        Decorative brass medallion shown on the door face.
  medallion.png

TO ADD A NEW OPTION (not just replace one):
1. Drop the new image file into the matching folder.
2. Open door-configurator.html in a text editor, find the `handles`
   or `laminates` array near the top of the <script> block.
3. Add a new line following the existing pattern, e.g.:
     { id:'l9', name:'Rosewood Dark', code:'L-09', img: LAM('your-file-name') }
   (omit the file extension inside LAM(...) / ICON(...) — .jpg / .png
   is added automatically)
