Magic Selection Techniques

1. Basic Selection

        Select Material:
        Command: :select
        Macro: s
        Function: Selects material under the cursor. Expands the selection based on the type of material.
        Examples:
            Single Material: Move cursor over a blue L-shaped area, press s to select the blue chunk.
            Expand Selection:
                Second Press: Includes all blue material in the region.
                Third Press: Selects the entire net connected to the initial selection.

        Add to Selection:
        Command: :select more
        Macro: S
        Function: Adds material to the existing selection.
        Example: Move cursor over a red bar and press S to add it to the current selection.


2. Area-Based Selection

        Select by Area:
        Command: :select area
        Macro: a
        Function: Selects all material within the defined box.
        Example: Draw a box around an area in tut2b and press a to select everything inside.

        Add by Area:
        Command: :select more area layers
        Macro: A
        Function: Adds material from specified layers within the box to the existing selection.
        Examples:
            :select area metal1 to select metal1 layer material.
            Follow with :select more area poly to add poly layer material.

3. Clearing Selections

        Clear All Selection:
        Command: :select clear
        Macro: C
        Function: Clears the current selection without affecting the selected material.
        Example: Press C to clear the current selection and start fresh.

        Deselect Portions:
        Command: :select less
        Function: Deselects material in the reverse order of selection.
        Command: :select less area layers
        Function: Deselects material from specified layers within the box.
        Examples:
            :select less to gradually deselect previously selected areas.
            :select less area metal1 to remove metal1 layer material within a new box.

4. Help and Synopsis

        Get Help on Selection:
        Command: :select help
        Function: Provides a summary of all selection options and commands.


selection operations you can perform:

        Action: Deletes everything within the selection.
        Macro: d
        Note: Different from :erase, which erases paint but keeps the selection box.

    [direction [distance]]
        Action: Moves both the box and the selection to a new location.
        Macro: t (for a simple move) or use directional arguments like :move up 10 to move precisely.
        Macros for directions: q (left), w (down), e (up), r (right)

        Action: Copies the selection and places the copy at the new location, leaving the original in place.
        Macro: c

    [direction [distance]]
        Action: Stretches the selection in a given direction while erasing paint along the path.
        Macro: T
        Directional macros: Q (left), W (down), E (up), R (right)

        Action: Flips the selection upside down.
        Note: The area occupied by the selection remains the same.

        Action: Flips the selection sideways.
        Note: Like :upsidedown, it maintains the total area of the selection.

    [degrees]
        Action: Rotates the selection clockwise. Degrees must be multiples of 90, defaulting to 90 if not specified.
        Note: The lower-left corner of the new selection aligns with the lower-left corner of the old selection.

Tips for Practice:

    Use :delete to remove selected elements and :undo to revert changes.
    Move elements around using :move or t. Try precise movements with directional commands.
    Practice copying elements with :copy or c.
    Experiment with :stretch (or T) to see how it affects the selected material.
    Flip selections using :upsidedown or :sideways and rotate with :clockwise.
