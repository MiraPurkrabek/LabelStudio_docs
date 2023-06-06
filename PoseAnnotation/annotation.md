# The annotation guide

The task of annotating 2D human pose involves identifying and marking key points on a person's body in an image. These key points correspond to important joints such as shoulders, elbows, wrists, hips, knees, and ankles. Your goal as an annotator is to accurately label these keypoints, enabling the understanding of the body's pose and movement for various applications like motion analysis, fitness tracking, and animation.

## Examples

There are some examples in this [file](examples.md)

## How to start

ToDo

## Annotation basics

After opening the application, you will see the first image from the dataset. Each image shows one person inside a rectangular box. If there are multiple people in the image, focus on annotating the person within the box. On the right side of the image, you will find a visualization of the annotation. Remember to mark the left side of the person as blue and the right side as yellow, orange, or red, even when the person is upside down or facing away.

To adjust the keypoints, use your mouse to click on a keypoint and drag it around the image. For more editing options, refer to the keyboard shortcuts provided below.

> __Joint location:__ The keypoint is where the joint rotates. It's around the middle of the limb, in terms of width.

### Keyboard Shortcuts

The pose annotation tool offers several keyboard shortcuts to improve your annotation workflow:

| Shortcut | Description                                                                                              |
| -------- | -------------------------------------------------------------------------------------------------------- |
| `u`      | **Next unannotated** pose                                                                                |
| `m`      | Save the current annotation progress and move to the **next one**                                        |
| `n`      | Save the current annotation progress and move to the **previous one**                                    |
| `v`      | Change the **visibility** of the currently selected keypoint (works only while holding the mouse button) |
| `d`      | **Delete** the currently selected keypoint (works only while holding the mouse button)                   |
| `a`      | **Add** a new kypoint, if one is missing                                                                 |
| `z`      | **Undo** the previous step                                                                               |
| `r`      | **Reset** the pose to the original                                                                       |
| `g`      | **Generate** a new pose                                                                                  |
| `l`      | **Flip L/R** of the pose                                                                                 |
| `q`      | **Quit** the program (with save)                                                                         |


### Annotated vs. Un-annotated images

If a person has already been annotated in the application, their bounding box will be displayed in a darker shade of green. You can still view previously annotated persons for later reference. To skip directly to the next unfinished task, press the 'u' key.

### Memory

The program remembers the steps you've taken, so you can go back to the way things were before. However, if you change the image or exit the program, this memory will be lost, and you won't be able to undo or reset your actions.

### Visibility

The visibility of keypoints is indicated by their transparency. Keypoints that appear with semi-transparent lines and a grey marker are annotated as non-visible. Make sure to accurately annotate the visibility for each keypoint. If you're unsure whether a keypoint is marked as visible or not, select it with the mouse and press 'v' to toggle its visibility. You will notice the difference in visibility afterward.

> __Visibility:__ The keypoint is visible if you can see the corresponding joint directly in the image.

If the keypoint is not visible and you can't estimate where it is (for example face when facing away), delete the keypoint. You can delete keypoint with keyboard shortcut 'd'.

## Common mistakes

Here is a short list of common error in the data:
- Face annotated as visible when the person is facing away
- Missing annotation of the limb (eg. wrist) when it is visible
- Wrong visibility of the limbs

## Exporting results

The application automatically saves your progress when you switch to another image or exit the application. Once the folder is complete, you can simply send the annotation file (usually named '_person_keypoints_val2017.json_') via email.