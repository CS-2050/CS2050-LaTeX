# Tables -- Using `Tabular`
<!-- ${{\color{gray}\textnormal{Click here for a regular table\:}}}$ _[link](multi-page%20tables.md)_ -->

_[Click here for `longtables` i.e. multi-page tables.](multi-page%20tables.md)_

`tabular` is the most straight forwards in my opinion for this.
 
It should be auto-imported so there isn't a need to use `\usepackage{tabular}`. 


Below is a template you can copy and paste in if you'd prefer, but it's good to understand how it works incase some issue comes up! E.g. if a character is accidently deleted.

```latex
\begin{tabular}{rc|c}
    \# & \textbf{Statement} & \textbf{Reason} \\
    \hline

    1.  & insert statement & insert reasoning \\
    2.  & ... &  \\
    .   & ... &  \\
    .   & ... &  \\
    .   & ... &  \\
\end{tabular}
```


## Character Meanings

| Expression | Functionality  | Additional Information |
| ---- | ---- | ---- |
| `\\`      | New line/row    | $\rightarrow$ even if you're in the middle column it'll jump to cell 0 of the next line |
| `&`       | Next column     | `&&` will skip the cell and leave it blank |
| `\hline`  | Horizontal line | Adds a horizontal line that helps create a `t` shape table |
| `\#`      | Hashtag         | Hashtags are special characters so the `\` indicates that we want a literal hashtag. This is optional I just like using it to denote the row count column. You could just leave this column blank. |





## Additional Character Meanings
These are specifically for the `{rc|c}` part of `\begin{tabular}`
| Character | Functionality | Notes |
| ---- | ---- | ---- |
| `r` | Adds a right-aligned column |  |
| `j` | Adds a justified column |  |
| `c` | Adds a centred-column |  |
| `\|` | Inserts vertical bar into table at this spot | The bar character between BACKSPACE and ENTER |
| `\|\|` | Inserts a double dividing bar |  |



### Character Examples
<table border="0">
 <tr>
    <td>
    r c c
    </td>
    <td>
    3 columns
    </td>
    <td>
    right, centred, centred
    </td>
 </tr>
  <tr>
    <td>
    j | c
    </td>
    <td>
    2 columns with a dividing bar
    </td>
    <td>
    justified, centred
    </td>
 </tr>
  <tr>
    <td>
    r r c || j l
    </td>
    <td>
    5 columns with a doublebar between the first 3 and last 2
    </td>
    <td>
    right, right, centred, BAR, justified, left
    </td>
 </tr>
</table>


<!-- Insert example of proof, of Big-O cause dif format, of truth tables, etc. -->
## Full Examples
<table border="0">
 <tr>
    <td>
    Code
    </td>
    <td>
    Output
    </td>
    <td>
    Notes
    </td>
 </tr>
  <tr>
    <td>
    j | c
    </td>
    <td>
    2 columns with a dividing bar
    </td>
    <td>
    justified, centred
    </td>
 </tr>

</table>