### Historical Context gramplet

![](./gramplet.png) 
Gramplet to display significant historical events with the year they happened (and optionally) the year they ended.

A double-click on a row will open a browser tab at the provided Link

The gramplet considers the lifespan of the Active Person in the People and the Relationship Category views splitbars.
It will use the birth and death of the active person to narrow the list to pertinent events. If either of the dates are missing the gramplet assumes a probable life span set in the Preferences using Gramps' "Probably Alive" calculation.
 
The data for the gramplet comes from a simple CSV file using the semi-colon delimiter, which can be edited with a normal text editor.

The Format is:

`from;to;event;link to event`

example:

`1789;1797;George Washington;https://wikipedia.org/wiki/George_Washington`

Dates can be written in any of Date formats normally uses, including "Today" for ongoing events.

The file name is `<locale>_data_v1_0.txt `e.g. `da_DK_data_v1_0.txt` for Denmark
Currently only a small assortment of files are provided, including `da_DK_data_v1_0.txt` and `en_US_data_v1_0.txt` which simply is a list of American presidents.

The third is `deafult_data_v1_0.txt` which will be used as a fallback, if there no data file if found for your language.

The fourth file is `custom_v1_0.txt`which can be used for adding your own data, which will be merged into the view.

You can add and use any semi-colon delimited file, as long as it ends with '_v1_0.txt´

## Options

The options can be accessed by the settings for the view:

![Options](./options1.png  "Options")

![Options](./options.png  "Options")

1 This string can be used to filter out text. If you set this to "Cen", then all lines where the text starts with "Cen" will be filtered out (i.e., "Census" as well as "Century", but not "1910 Census")

2 If you check this box, your filter will be active

3 This checkbox decides whether you will see all events or only those in your active person's life span

4. Whether you will use full dates or full years for comparison between the event and your active person's life span. This option also causes full dates to be displayed in the Gramplet.

5 The foreground color for lines within the active person's life span. There is a lot of applications, which let you convert a chosen colour to a HTML text string. I use KcolorChooser

6 The background colour for lines within the active person's life span
 
7  The foreground colour for lines outside the active person's life span

8 The background colour for lines outside the active person's life span

9 Files you choose to include in the timeline, Any files ending in `_v1_0.txt` will be listed, but it needs to hold data in the above format, in order to work.
