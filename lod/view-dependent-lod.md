# 

View-dependent LOD dynamically select the most appropriate level of detail for the current view.

## Naive

![](/assets/view_dependent_lod_distance.png)

---

## Anisotropic

Thus view-dependent LOD is _anisotropic_: a single object can span multiple levels of simplification. For instance, nearby portions of the object may be shown at higher resolution than distant portions. [Demo](https://jingbogit.github.io/engine.examples/earthLod/index.html) how Altizure Earth is anisotropic.

![](/assets/lod_anisotropic_close.png)

![](/assets/lod_anisotropic.png)

![](/assets/lod_anisotropic_far.png)

---

## Lod Forest

This leads to still better granularity: polygons are allocated where they are most needed within objects, as well as among objects. This in turn leads to still better fidelity for a given polygon count, optimizing the distribution of this scarce resource.















