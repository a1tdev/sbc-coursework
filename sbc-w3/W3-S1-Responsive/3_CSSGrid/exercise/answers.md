Answer 1: grid-template-areas lays out the defined areas in a 2 by 2 grid. Without this it breaks the layout.

Answer 2: 1fr will allow an item to take up all available space. Auto allows enough space for the content to exist. The fr unit takes precedence over the auto in the available space remaining.

Answer 3: Replacing 1fr with auto gives the 1st row more room

Answer 4:
.dashboard-container {
grid-template-areas:
"header"
"sidebar"
"main";
}

(or use a media query)

Answer 5: It adds a 10px gap to both the column and row. To add it to one or the other you add a second value e.g. gap: 10px 0;
