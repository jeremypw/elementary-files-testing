## Test cases for the item selection

### SELECT-01a
Select files (and only files) in the icon view and Miller column view

**Expected:** When the mouse is hovered over any of the selected files, an overlay is displayed at the bottom on the window with the selected file count and the sum of the file sizes

### SELECT-01b
Select files (and only files) in the icon view and Miller column view in the bottom end corner or the view and hover the mouse over the selection.

**Expected:** The overlay appears in the opposite corner, or moves to the opposite corner when the pointer enters it (continuing any ongoing count).

### SELECT-02a
Select two or more folders (and only folders ) in the icon view and Miller column view

**Expected:** When the mouse is hovered over any of the selected files, an overlay is displayed at the bottom on the window with the selected folder count

### SELECT-02b
Select one folder in the icon view and Miller column view

**Expected:** When the mouse is hovered over the selected folder, an overlay is displayed at the bottom on the window with the subfolder count and file count within the folder and the total size. An 'in progress' animation appears until the data is ready.

### SELECT-03
Select folders and files in the icon view and Miller column view

**Expected:** When the mouse is hovered over any of the selected files, an overlay is displayed at the bottom on the window with the selected folder count, the selected file count and the sum of the file sizes.

### SELECT-04
In Icon View and Column View, primary button down on white space and  drag diagonally.

**Expected:** A shaded rectangle appears and any icon touched by it is selected. Icons leaving the rectangle become deselected. Selection remains when button is released.

### SELECT-05
In List View, primary button down on white space in Filename column and  drag.

**Expected:** A shaded rectangle appears and any icon touched by it is selected. Icons leaving the rectangle become deselected. Selection remains when button is released.

### SELECT-06
In List View, primary button down on white space in Size, Type or Modified column and  drag.

**Expected:** No shaded rectangle appears. Only row initially clicked on is selected.

### SELECT-07
In any view, select some files.  Change to a different view.

**Expected:** The same files are selected in the new view.  If necessary the new view scrolls to show the selected file(s)

### SELECT-08
In Icon view, select a file.  Hold down the Shift key and use the Left and Right Arrow keys.

**Expected:** Further files are selected in a linear fashion, wrapping at the rightmost edge, completing one row before continuing at the start of the next.

### SELECT-09
In Icon view, select two adjacent files in a row, while holding the Shift key down.  Continue to hold down the Shift key and use the Up and Down Arrow keys.

**Expected:** Further files are selected in a linear fashion, completing one row before continuing at the start of the next. (Not in a rectangular fashion cf rubberbanding).

### SELECT-10
In Icon view of a folder containing enough files to fill several rows, starting from a position in the middle, press the right and left arrows without modifier.

**Expected:** Starting from the selected item the cursor position moves in a linear fashion, wrapping at the edges, and only the file under the cursor is selected.

### SELECT-11
In Icon view of a folder containing enough files to fill several rows, starting from a position in the middle, press the up and down arrows without modifier.

**Expected:** Starting from the selected item the cursor position moves upwards and downwards, not wrapping at the edges, and only the file under the cursor is selected. The view scrolls as required to keep the selected file in view.  If there is no file item beneath the current cursor position, the cursor does not move down.

### SELECT-12a
In all views of a folder containing multiple files, in single-click mode, select a contiguous set of files.  Click on the helper emblems of some selected files.

**Expected:**  Individual files are deselected, maintaining the selection of other files.

### SELECT-12b
In all views of a folder containing multiple files, in single-click mode, select a contiguous set of files.  Click on the helper emblems of some unselected files.

**Expected:**  Individual files are selected, maintaining the selection of other files.

### SELECT-13a
In all views of a folder containing multiple files, in single-click mode, select a contiguous set of files.  Click on the icon of selected files while holding down the control key.

**Expected:**  Individual files are deselected, maintaining the selection of other files.

### SELECT-13b
In all views of a folder containing multiple files, in single-click mode, select a contiguous set of files.  Click on the icon of unselected files while holding down the control key.

**Expected:**  Individual files are selected, maintaining the selection of other files.

### SELECT-14
In all views of a folder containing multiple files, select some files.  Press the up and down arrows while holding down the control key.

**Expected:**  The cursor moves (prelit icon) but the selection does not change.
