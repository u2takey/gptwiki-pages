# nms 
## chatgpt 
As an AI language model, I assume the command is related to object detection in computer vision. In the context of object detection, NMS stands for Non-Maximum Suppression. Non-Maximum Suppression is a technique used to filter duplicate object detections in an image.

The objective of object detection is to identify the location of objects in an image, with a bounding box around each object. Object detection models usually generate multiple proposals for detecting an object based on different features extracted from the image. However, these proposals can overlap or have similar scores if the object is present in the image in different orientations or scales. Non-Maximum Suppression identifies the highest score proposal, which is most likely to be the reliable detection, and suppresses the redundant proposals near it. This eliminates duplicate detections and ensures that there is only one bounding box marked per object.

The NMS algorithm works by sorting all of the bounding box proposals by their associated confidence scores. Starting from the bounding box with the highest score, it removes any box that has an intersection-over-union (IoU) value greater than a predefined threshold with any previously selected high-scoring bounding box. The remaining bounding boxes are then returned as the final object detections. The threshold value is usually set between 0.3 and 0.5 depending on the application.

The command nms is used to implement Non-Maximum Suppression in object detection applications. It typically takes as input a set of bounding box proposals, their corresponding confidence scores, and the defined overlap threshold. The output is a filtered set of non-overlapping bounding boxes with high confidence scores, representing the detected objects in the image. 

## tldr 
 
> Command-line tool that recreates the famous data decryption effect seen in the 1992 movie Sneakers from `stdin`.
> More information: <https://github.com/bartobri/no-more-secrets>.

- Decrypt text after a keystroke:

`echo "{{Hello, World!}}" | nms`

- Decrypt output immediately, without waiting for a keystroke:

`{{ls -la}} | nms -a`

- Decrypt the content of a file, with a custom output color:

`cat {{path/to/file}} | nms -a -f {{blue|white|yellow|black|magenta|green|red}}`

- Clear the screen before decrypting:

`{{command}} | nms -a -c`
