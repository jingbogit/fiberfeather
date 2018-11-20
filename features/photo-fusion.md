# Photo Fusion

---

The reconstructed model

* has defects. \(holes, corrupted water surface, glass surface, etc.\)
* The texture is not as vivid and high-res as the photos.
* thin structure like light poles, electrical wire cable can not be reconstructed.

![](/assets/features_photo_fusion_thin_structure_defect.png)

---

### 

### Solution:

Snap to the nearest view where a photo is taken. Cover the 3D model with that photo. Because the photo can nicely align with the view, it looks like the model suddenly improves to a high-res quality.

### nearby

1. **euclidean distance**: the distance between the current viewpoint and the photo taken point.
2. **orientation difference**: the angle between the view and the photo's looking direction.

A weighted sum of these two difference is used as the distance score.  There will be no nearby photo if the minimum score is higher than a threshold. In that case, a red dot will be shown at the center of the screen. On the contrary, current view will snap to that photo, and a green dot will show.

### Control mode

1. normal control.

2. snapped mode is activated after a nearby photo is found. Left button will move the photo, mouse wheel will enlarge/shrink the photo. The photo will align with the background model at all time.

3. The de-activation of the snapped mode happens in two cases:

         3.1. the center of the screen is at the very edge of the photo, move further will cause the photo out of screen.

         3.2. Mouse right button rotate. the view direction is  changed, need to look for another photo.

---

### Distortion

To align the model with the photo, we changed the camera's fov and view-port. It will distort the model, which is normal and expected.

