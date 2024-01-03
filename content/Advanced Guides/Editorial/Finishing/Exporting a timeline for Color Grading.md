---
title: Exporting edits for Color Grading
tags:
  - Color
---
###### STEP 1 - EXPORT A REFERENCE

In Premiere, export a reference video of the approved edit as QuickTime ProRes LT to 02_Assets/05_Color/00_ColorPrep. Add the suffix “\_PicRef”. See page 3 & 4 for details.

###### STEP 2 - PREPARE THE SEQUENCE

A – Duplicate the approved sequence(s) and add the suffix “\_ColorPrep”. Use this to prepare the files.

B – Take note of how many frames each transition takes up before they are removed in the next step. Either request from the colorist the correct number of frame handles (extra frames before and after each cut) or manually lengthen the footage.

C – In “\_ColorPrep” timeline(s), collapse it to as few video tracks as possible and remove unneeded elements (audio, graphics, overlays, etc). This can be done manually. Or use Sequence > Simplify Sequence and check all the boxes for automatic removal.

D – Un-nest any sequences and flatten Multi-Camera Sequences. Highlight all clips, right click, and choose “Remove attributes.” Uncheck “Time Remapping” as this will need to be removed clip by clip to ensure ripple edits.

IN CAMERA ATTRIBUTES:  
All in-camera color LUTs must be removed from the source clip in the “Source Effects” panel under “Effect Controls”. This can be done on most clips by right clicking on the contents of a bin of media and choosing “Disable Source Clip Effects.” Clips with source effects will have a red line under the FX badge.

E – Remove all speed duration changes or any keyframes from clips.

SPEED NOTE:  
During the edit process, it is recommended to nest any clips before adding time remapping keyframes or any flat speed % adjustments (e.g., 200%). This will ensure that there are no speed interpolation/frame rate issues once the graded clips are received back from the colorist.

F – Highlight all clips, right click, and select “Set to Frame Size.”

G – All remaining clips that do not have a gray “fx” box in the corner must be looked at individually to remove any other effects.

###### STEP 3 - EXPORT XML

Select the sequence, and export to the 00_ColorPrep folder using “File > Export > Final Cut Pro XML”. If there are multiple rounds of prep, make subfolders with dates. If any elements can’t be translated, a text file report will be placed next to the XML so you can review timecodes of clips that have issues.

###### STEP 4 - EXPORT XML REFERENCE

Then, export the same timeline that matches the XML exactly for the colorist as QuickTime ProRes LT. Export to the same ColorPrep folder and add the suffix “\_ColorXMLRef”.

###### STEP 5 - OUTSIDE COLORIST

If working with an outside colorist, prepare the raw files to send along. IMPORTANT: Complete the detailed steps in the next section, page 12, before proceeding.

When working with an outside colorist, the source files need to collected, and sometimes trimmed. Use the Premiere method when there are fewer or small files. Use DaVinci Method when there are large files, especially files that need to be trimmed.

PREMIERE METHOD:

Within Premiere, navigate to File > Project Manager. Select the correct sequences. Click Browse and choose the destination “02_Assets/05_Color/00_ColorPrep”. Click ‘OK’

DAVINCI METHOD:

A - Open up Davinci Resolve and import your XML using File > Import > Timeline > (choose your XML file). Once imported, scrub the timeline to make sure it looks correct.

B - Navigate to File > Media Management. In the new dialogue box....

DaVinci Resolve

- Select the top “Entire Project.”
- Make sure you’ve selected “Copy” and not “Transcode.”
- Select, “Used media and trim.”
- Type in the number of frame handles needed (e.g. 24).
- Select Browse and create a subfolder in “00_ColorPrep” called “SourceMedia”.
- Click “Start” and let the program run. You should start seeing new files populating in the SourceMedia folder.