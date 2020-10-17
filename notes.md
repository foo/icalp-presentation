* technical questions
** beamer? or something better, maybe web-based?
** figures? IPE? Krita?
*** Handmade + photos? (hard to change)

* technicalitios
** audacity filters?


Slides sketch
* model
    * quick results in the model:
        * no competitiveness of one bucket
        * some example to emphasize that we maximize
    * visualization of buckets forming a line
* result
    * 0.6* (*roughly)
    * it is tight, and randomized lower bound of Jez

* our algorithm
    * large, medium and small, różne kolory
    * wizualizacja, po ile się mieszczą

* large items only are interesting already
    * taking all => 0.5 < 0.6
        * adversary inserts 1's when we run out of buckets
    * rejecting?
        * adversary ends the sequence and collects all
    * our solution: Rising Threshold Algorithm
        * until n*0.6'th bucket, we accept all
        * then, we start to be more picky
        * the threshold function
        * properties of threshold function

* large and medium items
    * large respecting
        * if we take all medium, and larges according to the threshold, and the we have buckets left, then we are fine
    * so, let's take all medium
        * pile in own buckets? not enough, even if we combine with larges
        * keep separated, with hopes to combine? what if larges never come?
    * our solution: keep some together, and keep some isolated
        * how many? no universal answer : it depends on actual sizes of items
        * a structure D
        * we analyse our algorithm in terms of the minimum tight item, i.e., the minimum among these almost touching the function, as only them "let out" of the structure certain element

* end: thanks for my phd supervisor, Marcin Bienkowski
