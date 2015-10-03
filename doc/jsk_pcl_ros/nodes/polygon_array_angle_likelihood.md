# PolygonArrayAngleLikelihood
Compute likelihood based on distance.
Near polygon is, larger likelihood is.
The likelihood is determined by `1/(1+d^2)` where `d` is a angular difference from `~target_frame_id` to the polygon.

## Subscribing Topic
* `~input` (`jsk_recognition_msgs/PolygonArray`)

  Input polygon array.

## Publishing Topic
* `~input` (`jsk_recognition_msgs/PolygonArray`)

  Input polygon array.

## Parameters
* `~target_frame_id` (required)

  Frame id to compute polygon's distance from
* `~tf_queue_size`

  Queue size of tf message filter