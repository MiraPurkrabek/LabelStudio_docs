
**Keypoint visibility**

| Value | Appeareance                           | Definition                                     | Example                                                                         |
| ----- | ------------------------------------- | ---------------------------------------------- | ------------------------------------------------------------------------------- |
| 0     | No keypoint, no bones                 | No information, keypoint can be anywhere       |                                                                                 |
| 1     | Grey keypoint with semi-visible bones | Location of keypoint precise but not visible   | [Example](images/visibility_1.png)                                              |
| 2     | Fully visible keypoint and bones      | Keypoint is clearly visible                    | [Example](images/visibility_2.png)                                              |
| 3     | No keypoint, semi-visible bones       | Location of keypoint approaximate, not visible | [Example 1](images/visibility_3.png) and [Example 2](images/visibility_3_1.png) |


**Keypoint localization**

If the keypoint is not in the image, we estimate it's location in the grety strip around the image. The scale of the gray area is **exponential** so that the first line (in the middle of the script) corresponds to distance of half of the image, second line distance of the image and so on.

| Line | Scaled distance from the border of the image | Real distance from the border of the image |
| ---- | -------------------------------------------- | ------------------------------------------ |
| 1    | 1/2 of the image width/height                | 1/2 of the strip width/height              |
| 2    | 2/2 of the image width/height                | 3/4 of the strip width/height              |
| 3    | 3/2 of the image width/height                | 7/8 of the strip width/height              |
