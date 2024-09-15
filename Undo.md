# Undo and Redo Commands

    Undo:
        Command: :undo
        Macro: u
        Function: Reverts the effects of the most recent command. You can use it multiple times to undo several commands, but Magic can only remember the last ten or so commands for undo purposes.

    Redo:
        Command: :redo
        Macro: U
        Function: Reapplies the command that was undone. Useful if you change your mind after an undo and want to restore the previous state.

# Practical Use

    Experiment with Commands:
        Make some changes by painting and erasing.
        Use the :undo command (or u macro) to revert these changes one step at a time.
        Observe how each undo affects your layout to understand the impact of each command.

    Redo After Undo:
        After undoing a command, use :redo (or U macro) to reapply the undone changes if you decide you want them back.

    Undo Limitations:
        Remember that Magic keeps track of a limited number of commands for undo (usually the last ten). If you exceed this limit, older commands will no longer be available for undo.

    Practice Sequence:
        Try a sequence of paint and erase operations.
        Undo each step to see how it affects your layout.
        Redo steps to ensure you understand how the redo command restores the previous state.

# Example Workflow

    Initial Actions:
        Paint a few layers.
        Erase some parts.

    Undo Actions:
        Use :undo to revert the most recent changes.
        Continue using :undo to step back through your changes.

    Redo Actions:
        After undoing, use :redo to reapply changes.
        Ensure that the :redo command brings back the exact changes you reverted.
