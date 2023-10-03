# Module-CrestronSourceNameSearch


        ___     ________        * * * * * * * ====================
       |\  \   |\   ____\        * * * * * *  ====================
       \ \  \  \ \  \___|       * * * * * * * ====================
     __ \ \  \  \ \  \  ___      * * * * * *  ====================
    |\  \\_\  \  \ \  \|\  \    * * * * * * * ====================    __
    \ \________\  \ \_______\   ==================================  <(o )___
     \|__1776__|   \|_______|   ==================================   ( ._> /
                                ==================================    `---' 

This was built because I had to make a module that would search through an NVX system that had 500 sources...

The Module is structured this way:

     INPUTS
     STRING    Search$
     DIGITAL   Source[001-500]VIS_IN
     STRING    Source[001-500]Text$

     OUTPUTS
     STRING    Search_FB$
     DIGITAL   Source[001-500]VIS_OUT

I tied "Search$" to the TextEntry smart graphic on my touch panel. For every change of this string, the module
will perform a FOR loop to check each "Source[X]Text$" that is also shown high for "Source[X]VIS_IN". If there is a match
then "Source[X]VIS_OUT" goes high.

When the length of "Search$" is 0, then "Source[X]VIS_OUT" is set equal to "Source[X]VIS_IN".

I wanted to make this a C# module, but not sure how to do that right now. If you know of a solution

Enjoy!
