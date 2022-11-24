# Annotation examples

Here I present some examples of correct and wrong annotation. Each image has its description. You can click images to their full size.

## Which player annotate

These images show which players are to be anotated. Select only those players with known identity and give players the proper color. Goalie is t be annotated the same color as its team. Examples are shown in pictures below.

<p float="middle">
  <img src="imgs/correct_annotation_before.png" width="300" />
  <img src="imgs/correct_annotation_after.png" width="300" />
</p>

And one more in the zommed situation.

<p float="middle">
  <img src="imgs/correct_annotation_close_before.png" width="300" />
  <img src="imgs/correct_annotation_close_after.png" width="300" />
</p>

## How to draw a rectangle

The rectangle should be close fit for the player. The edges should touch its body parts. In other word, the rectangle should be as small as possible while having the whole player inside.

The player is only the body, not the stick. The **correct example** is shown below.

![](imgs/bbox_correct.png)

### Wrong rectangles

Now I show common errors while drawing rectangles. The errors are:

- a) The head is not in the rectangle - rectangle too small.
- b) The feet is not in the rectangle - rectangle too small.
- c) The rectangle is too big.

<p float="middle">
  <img src="imgs/bbox_wrong1.png" width="300" />
  <img src="imgs/bbox_wrong2.png" width="300" />
  <img src="imgs/bbox_wrong3.png" width="300" />
</p>

