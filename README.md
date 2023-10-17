[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/Y8Y7PSI74)
# __Searching Source Names to present on the Touch Panel__ 


      __         __         __         __         __         __
    <(o )___   <(o )___   <(o )___   <(o )___   <(o )___   <(o )___     GOD BLESS AMERICA
     ( ._> /    ( ._> /    ( ._> /    ( ._> /    ( ._> /    ( ._> /     JULY 4TH, 1776
      `---'      `---'      `---'      `---'      `---'      `---' 
## What does this module do?                                   

This was built because I had to make a module that would search through an NVX system that had 500 sources...

The Module is structured this way:
| TYPE     | INPUT VAR             | OUTPUT VAR             | TYPE     |
|--------: | --------------------: | :--------------------- | :------- |
| STRING   | Search$               | Search_FB$             | STRING   |
| DIGITAL  | Source[001-500]VIS_IN | Source[001-500]VIS_OUT | DIGITAL  |
| STRING   | Source[001-500]Text$  |                        |          |

### How it works...
*I tied "Search$" to the TextEntry smart graphic on my touch panel.* 

1. For every change of __Search$__, the module will perform a FOR loop to check each __Source[X]Text$__, however, it will only check the source text of sources that are also __*Enabled*__ via __Source[X] VIS_IN__. 
1. If there is a match then __Source[X]VIS_OUT__ goes high.
1. When the length of __Search$__ is __0__, then __Source[X]VIS_OUT__ is set equal to __Source[X]VIS_IN__.

I wanted to make this a C# module, but not sure how to do that right now. If you know of a solution let me know in [This Discussions](https://github.com/Duck1776/Module-CrestronSourceNameSearch/discussions/1)

__*Enjoy!*__

## TO-DO
- [X] PROVIDE MODULE
- [ ] PROVIDE EXAMPLE PROGRAM
- [X] DETAIL README

---
<br>

[![Duck1776 GitHub stats](https://GitHub-readme-stats.vercel.app/api?username=Duck1776)](https://GitHub.com/anuraghazra/GitHub-readme-stats) 

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/Y8Y7PSI74)