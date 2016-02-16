I often find myself scrolling with the mouse wheel far back into a buffer, and then selecting something with the mouse in order to copy something with command+c. When I release the mouse button, tmux exits copy mode and jumps to the bottom of the buffer.

After search how to prevent this problem with google, I find that there is no need to do that, because tmux has some fairly good scroll and search keyboard mappings by default for copy mode.

> space starts selection and enter copies

Function              | vi
--------------------- | --
Start selection       | Space
Copy selection        | Enter
Clear selection       | Escape
Cursor to middle line | M
Cursor to top line    | H
Half page down        | C-d
Half page up          | C-u
Next page             | C-f
Previous page         | C-b
Search backward       | ?
Search forward        | /
