# Troubleshooting Guide

This guide covers the most common issues you may run into while following the Non-Destructive Editing and Vector Shapes tutorials, along with detailed steps to fix each one.

---

## 1. The Layers Panel Is Not Visible On Screen

If you cannot see the Layers panel, you will not be able to duplicate your Background layer, add Adjustment Layers, or manage Smart Objects, all of which are required for these tutorials.

**Fix:**

1. Go to **[Window]** in the top menu bar
2. Click **[Layers]** - the Layers panel will appear on your screen
3. If it opens as a floating panel, drag it toward the right edge of your screen until it attaches and stops floating

!!! note
    You will know it worked when you can see a panel on the right side of your screen showing a row labelled **Background** with a small padlock icon next to it.

---

## 2. The Shape Tool Is Drawing a Path Outline or Flat Pixels Instead of a Scalable Vector Shape

After drawing your shape, it appears either as a thin outline with no fill, or as a flat coloured area you can no longer resize or edit. This happens because the mode is set to **Path** or **Pixels** instead of **Shape**.

**Fix:**

1. Look at the horizontal bar that runs along the very top of your screen, just below the menu bar - this is the options bar
2. On the far left of that bar, you will see a dropdown that reads either **Shape**, **Path**, or **Pixels**
3. Click it and select **Shape**
4. If you have already drawn your shape incorrectly, press `Ctrl + Z` to undo, change the mode to **Shape**, and redraw it

!!! note
    You will know it worked when small blue anchor points appear at the corners and edges of your shape after you release the mouse.

---

## 3. The Pen Tool Creates a New Anchor Point Instead of Closing the Shape

When you try to close your path, clicking near the first anchor point places a new point instead, leaving your shape open and unfilled.

**Fix:**

1. Hover your cursor very slowly and precisely over the exact first anchor point you placed
2. Watch closely for a **small circle icon** to appear next to the pen cursor, this is the only visual signal that Photoshop is ready to close the path
3. Do not click until you see that circle
4. If you clicked too early and created an extra point by mistake, press `Ctrl + Z` immediately to undo, then hover over the first point again more carefully before clicking

!!! note
    You will know it worked when your shape becomes a fully enclosed, filled area with no open gaps or loose lines.

---

## 4. Gaussian Blur Appears as a Permanent Change Instead of an Editable Smart Filter

After applying **[Filter] → [Blur] → [Gaussian Blur]**, the blur is applied directly to the layer with no Smart Filter appearing underneath it in the Layers panel. This means the layer was not converted to a Smart Object before the filter was applied.

**Fix:**

1. Press `Ctrl + Z` to undo the blur
2. In the Layers panel, right-click your layer and select **[Convert to Smart Object]** - you will know the conversion worked when a small square icon appears on the small image preview square on the left side of your layer row
3. Reapply the filter via **[Filter] → [Blur] → [Gaussian Blur]** and click **[OK]**

!!! note
    You will know it worked when the words **Gaussian Blur** appear as a separate, clickable line directly below your layer in the Layers panel. You can double-click that line at any time to adjust the blur radius.

---

## 5. All Layers and Edits Are Lost After Saving

After reopening your file, everything appears flattened into a single image - all Adjustment Layers, Smart Objects, and Smart Filters are gone and can no longer be edited.

**Fix:**

1. Always save your working file via **[File] → [Save As]**
2. Set the format to **Photoshop (.psd)**
3. Click **[Save]**

!!! note
    You will know it worked when you reopen the file and can still see all your individual layers listed separately in the Layers panel, rather than a single flattened image.

!!! warning
    Saving as `.jpg` or `.png` permanently flattens all layers into pixels and cannot be undone. Only export to `.jpg` or `.png` when you have a fully finished version that you no longer need to edit - and even then, always keep your `.psd` file as your master copy.

---

## 6. A Warning Triangle Icon Appears Next to My Selected Color in the Color Picker

While selecting a fill color for your shape in the Color Picker, a small triangle with an exclamation mark (⚠️) appears next to your chosen color. This can look alarming, but it is not an error, it is Photoshop's **out-of-gamut warning**, which means the color you have selected may not print accurately on a physical printer.

**Fix:**

1. If you are working on a **digital project** (anything viewed on a screen), you can safely ignore this warning entirely, it has no effect on how your color looks on screen
2. Simply click **[OK]** to confirm your color selection and continue

!!! note
    You will know everything is fine when the Color Picker closes and your chosen color appears correctly in the **Fill** box in the top options bar, ready for you to draw your shape.
