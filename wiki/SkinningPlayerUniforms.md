# How to Skin Player Uniforms

**Applies to:** RotU 2.2.2 and later (r130+).  
The same general process also works for RotU 2.2.1, though the images and models are slightly different.

## Introduction

The player uniform skinning masks are located in `src/skins/players`.  
These are native **GIMP `.xcf`** files, with the masks stored as channels inside each image.  

You **must** have the **GIMP DDS Plugin** installed to export the textures correctly.

## Step-by-Step Guide

1. Create a **2048×2048 pixel** image of the camouflage pattern you want to use.

2. Open the uniform image you want to skin in **GIMP**.

3. Go to **File → Open as Layers...** and select your camouflage image.

4. Make a copy of the original uniform layer and move it to the **bottom** of the layer stack.  
   **Important:** The original uniform layer **must** be the bottom layer, or the final texture will not work correctly.

5. Hide all layers except the camouflage layer.

6. Switch to the **Channels** tab, right-click on the **Quick Mask**, and select **Mask to Selection**.

7. Switch back to the **Layers** tab. Make sure the camouflage layer is visible and active, then go to **Edit → Copy**.

8. Go to **Edit → Paste As → New Layer**.

9. Make all layers visible again. Adjust the layer order as needed until the uniform looks correct, ensuring the original uniform layer remains at the bottom.

10. **File → Save** to save your `.xcf` project.

11. Go to **Image → Merge Visible Layers...** and choose **Clipped to bottom layer**.

12. **File → Export...** and save the image with the original filename but with a `.dds` extension.  
    Use these export settings:
    - **Compression**: BC3 / DXT5
    - **Mipmaps**: Generate Mipmaps

13. **Edit → Undo** "Merge Visible Layers" (to restore your layered version if needed).

14. Convert the exported `.dds` file to `.iwi` format using an image converter tool.

15. Collect all the resulting `.iwi` files and package them into an `.iwd` file as usual.

## Editing the Masks (Optional)

If the built-in masks aren't quite right, you can edit them directly:

- Select the mask channel in the **Channels** tab.
- Paint on the mask using the paint tools:
  - **Pure white** = erases part of the mask (this area will show the camouflage).
  - **Pure black** = makes the area opaque (this area will **not** be camouflaged).
  - **Grayscale values** = create semi-transparent transitions.

---

*Originally ported from the Google Code wiki.*