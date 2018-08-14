## Trade-offs:

* **Massive data** \(up to TB level\) vs. **hardware capability** \(internet bandwidth, RAM, etc.\)

* **fidelity** vs. **frame rate**



---

## 

## General idea of Level of Detail \(LOD\)

A complex object is simplified. We call the original object as the _highest level_, the simplest one as the _lowest level_.

Lower levels cost less memory, and is faster to download.

![](/assets/view_dependent_lod_triangles.png)

Creating levels of detail or LODs to reduce the rendering cost of small, distant, or unimportant geometry.

![](/assets/view_dependent_lod_distance.png)

