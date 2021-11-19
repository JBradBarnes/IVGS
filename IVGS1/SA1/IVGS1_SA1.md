# IVGS1_SA1 
## - Specification class for a Sprite Assembly

A sprite assembly is a collection of sprites organized by directional view sets.

Each assembly shall be made up of component sprites with a definition of parenting and anchors to rotate individually around or move about on the x or y axis.

Sprite data shall define its rectangular envelope with x, y properties and its rotation anchor with anchor_x and anchor_y.

When a parent is rotated the children should additionally be rotated around the parent's anchor. 
