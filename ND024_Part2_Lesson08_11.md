# Lesson 8.11 Quiz: Strategy Quiz 2

Scenario: You've Developed a self-publishing website where people post a single image with a comment.

Questions:
1. Convert to vector or keep as JPEG
2. inline images or set their sources to external files?

Solution:
1. Keep as JPEGs. These are raster so keep in raster
2. To access on mobile, keep inline if you can, to reduce number of requests browser has to make.
Requests add rountrips, and roundtrips are slow for websites.
However, in the next lesson, we see that inline images limit your responsive options, so in the end, an external file might be the answer.  Therefore, either answer here is correct.

- - -
Next up: [Quiz: Strategy Quiz 3](ND024_Part2_Lesson08_12.md) or return to [Table Of Contents](./ND024_TableOfContents.md)
