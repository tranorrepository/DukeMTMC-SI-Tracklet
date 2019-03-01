# DukeMTMC-SI-Tracklet

DukeMTMC-SI-Tracklet [1] is an auto-detected tracklets subset of the [DukeMTMC](http://vision.cs.duke.edu/DukeMTMC/) tracking dataset [2] for video-based person re-identification.

We built this new tracklet person re-id dataset as follows. We first deployed an efficient deep learning tracker that leverages a COCO+PASCAL trained SSD for pedestrian detection and an ImageNet trained Inception for person appearance matching. Applying this tracker to all DukeMTMC raw videos, we generated 19,135 person tracklets. Due to the inevitable detection and tracking errors caused by background clutters and visual ambiguity, these tracklets may present typical mistakes (e.g.ID switch) and corruptions (e.g. occlusion).

We finally obtained 12,647 person tracklets from 1,788 unique IDs. To match DukeMTMC-VideoReID [3], we set the same 702 training IDs with the remaining 1,086 people for performance test (missing 14 test IDs against DukeMTMC-ReID due to tracking failures).

### Download Dataset
You can download the DukeMTMC-SI-Tracklet dataset from
[[Google Drive]](https://drive.google.com/open?id=1JR7z3sCyCC23nziYHDATClJwnCW39z5b)

### References
- [1] Minxian Li, Xiatian Zhu, Shaogang Gong. Unsupervised Tracklet Person Re-Identification. TPAMI 2018.

- [2] Ristani, Ergys and Solera, Francesco and Zou, Roger and Cucchiara, Rita and Tomasi, Carlo. Performance Measures and a Data Set for Multi-Target, Multi-Camera Tracking. ECCVWS 2016.

- [3] Wu, Yu and Lin, Yutian and Dong, Xuanyi and Yan, Yan and Ouyang, Wanli and Yang, Yi. Exploit the Unknown Gradually: One-Shot Video-Based Person Re-Identification by Stepwise Learning. CVPR 2018.

Please cite the following two papers if this dataset helps your research.
```
@inproceedings{
  title = {Unsupervised Tracklet Person Re-Identification},
  author = {Minxian Li, Xiatian Zhu, Shaogang Gong},
  booktitle = {Accepted to appear in IEEE Transactions on Pattern Analysis and Machine Intelligence},
  year = {2018}
}

@inproceedings{ristani2016MTMC,
  title = {Performance Measures and a Data Set for Multi-Target, Multi-Camera Tracking},
  author = {Ristani, Ergys and Solera, Francesco and Zou, Roger and Cucchiara, Rita and Tomasi, Carlo},
  booktitle = {European Conference on Computer Vision workshop on Benchmarking Multi-Target Tracking},
  year = {2016}
}

@inproceedings{wu2018cvpr_oneshot,
  title = {Exploit the Unknown Gradually: One-Shot Video-Based Person Re-Identification by Stepwise Learning},
  author = {Wu, Yu and Lin, Yutian and Dong, Xuanyi and Yan, Yan and Ouyang, Wanli and Yang, Yi},
  booktitle = {The IEEE Conference on Computer Vision and Pattern Recognition (CVPR)},
  month = {June},
  year = {2018}
}
```