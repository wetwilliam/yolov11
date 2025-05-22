# Changelog


## [2025-05-22]
Modify from official main commit:
 [a2b1c3d4e5f678901234567890abcdef12345678] (Remove `frozenset` from `ValueError` logs (#20746))

### Added


- Added `RandomHDRTone` class to `ultralytics/ultralytics/data/augment.py` for simulating HDR tone mapping.
- Integrated `RandomHDRTone` into `ultralytics/ultralytics/data/augment.py::v8_transforms` with configurable parameter (`hdr_tone`).
- Added `hdr_tone` hyperparameter to `ultralytics/ultralytics/cfg/default.yaml`.
- Added `RandomLightSource` class to `ultralytics/ultralytics/data/augment.py` for simulating light source augmentation.
- Integrated `RandomLightSource` into `ultralytics/ultralytics/data/augment.py::v8_transforms` with configurable parameters (`lightsource`, `lightsource_max_brightness`, `lightsource_min_radius_factor`, `lightsource_max_radius_factor`).
- Added `lightsource`, `lightsource_max_brightness`, `lightsource_min_radius_factor`, and `lightsource_max_radius_factor` hyperparameters to `ultralytics/ultralytics/cfg/default.yaml`.

### Changed

- Set `hsv_h`, `hsv_s`, and `hsv_v` to 0.0 in `ultralytics/ultralytics/cfg/default.yaml`.