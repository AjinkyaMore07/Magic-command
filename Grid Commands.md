Grid Commands

    :grid [spacing]
        Action: Toggles the grid on/off or sets the grid spacing.
        No arguments: Toggles grid visibility.
        Single numerical argument: Sets grid spacing (e.g., :grid 5 sets spacing to 5 units).
        Two arguments (xSpacing ySpacing): Sets different spacings for x and y axes.
        Four arguments (xSpacing ySpacing xOrigin yOrigin): Sets spacings and a reference point for the grid.
        :grid off: Turns the grid off.
        Macros:
            g for :grid (default spacing of 1 unit).
            G for :grid 2 (spacing of 2 units).

Zoom and View Commands

    :zoom factor
        Action: Adjusts the zoom level.
        Example: :zoom 2 zooms out so that twice as many units are visible. :zoom .5 zooms in to show half as much of the layout.
        Macro: Z

    :findbox [zoom]
        Action: Centers the view on the selected box and optionally adjusts the zoom to make the box nearly fill the screen.
        Macro: z (with zoom) or B (without zoom).

    :view
        Action: Resets the view to show the entire cell.
        Macro: v

Box and Measurement Commands

    :box
        Action: Prints out the size and location of the selection box.
        Macro: b
        Additional Use: Can also be used to set the box dimensions and location. Check the man page for detailed syntax.

Selection Information

    :what
        Action: Prints information about the currently selected items, such as their layer or type.

Macro Commands

    :macro [char]
        Action: Prints the long command associated with a macro. If char is omitted, it lists all macros.
        Example: :macro 1 shows the command for the 1 key macro.

    :macro char command
        Action: Sets a macro (char) to a specific command (command). Enclose commands with spaces in double-quotes.
        Example: :macro 1 "echo You just typed the 1 key."

    . (dot macro)
        Action: Repeats the last command you typed.

Usage Tips

    Use the grid to align and place elements accurately.
    Zoom in and out to work on different scales or get a better view of your layout.
    Use :view to quickly reset and see the entire cell.
    Use :what to gather details about selected elements, which is useful for troubleshooting and verification.
    Set up custom macros for frequently used commands to streamline your workflow.

