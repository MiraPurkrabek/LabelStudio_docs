# Data log

This file describes/documents data used for the project. Data can be in five stages. The stages corresponds to the folders in the data cluster.

1. Selected
    - Data selected (and noted in this log) for annotation
2. Ready
   - Data prepared for the annotation but not given to the annotator
3. WIP
    - Data given to the annotator for the annotation
4. Review
    - Annotated data waiting for review and processing
5. Done
    - Annotated, reviewed and processed data


## Selected

The table below logs sequences selected as suitable for annotation.

| Sequence name                 | Length  | N° subparts      | Extras (why selected) |
| ----------------------------- | ------- | ---------------- | --------------------- |
| MA_SKV_HAT_24_10_2021_T.mp4   | 1:53:04 | 6                |                       |
| MA_SKV_SPA_17_08_2021_T.mp4   | 1:41:25 | 5 (1:25 missing) |                       |
| U19_SKV_BUD_17_11_2021_T.mp4  | 1:58:55 | 6                |                       |
| U19_SKV_CHOM_24_10_2021_T.mp4 | 1:52:02 | 6                | Strong sun            |
|                               |         |                  |                       |

## Ready

To mark sequence as ready, it has to:

1. Be cut into 20 min sequences with 20 fps
2. Be pre-processed (extracted frames and subclips) by the [script](scripts/extract_random_frames_with_video.py).
3. Be available in the appropriate folder in the cluster
4. Be zipped for easier download

| Sequence name                    | Length  | N° subparts            | Extras (why selected)                          |
| -------------------------------- | ------- | ---------------------- | ---------------------------------------------- |
| MA_SKV_MB_31_10_2021_T.mp4       | 1:43:51 | 5 (3:51 missing)       |                                                |
| MA_SKV_PCE_10_03_2022_T_full.mp4 | ------- | 3 (Warmup and 2 match) | Warmup (12:33 - 17:33), match (41:48, 1:01:48) |
|                                  |         |                        |                                                |

## WIP

This is the overview of sequences already in process of annotation.

| Sequence name | Length | N° subparts | Extras (why selected) |
| ------------- | ------ | ----------- | --------------------- |
|               |        |             |                       |

## Review

This is the overview of sequences already annotated and waiting for review.

| Sequence name | Length | N° subparts | Extras (why selected) |
| ------------- | ------ | ----------- | --------------------- |
|               |        |             |                       |

## Done

This is the overview of sequences already annotated, reviewed and post-processed. The post-processing consists of:

1. Save annotations in some common format
2. Save both frames and annotation in the cluster

| Sequence name | Length | N° subparts | Extras (why selected) |
| ------------- | ------ | ----------- | --------------------- |
|               |        |             |                       |
