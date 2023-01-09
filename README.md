# ILC Dataset

We release some data sample in the folder `data`. The collectors use their smartphones to scan the features (e.g., BLE signals) as the location fingerprints, and the data are saved in the trace files. The structure of `data` is shown as follows.

```
\---site1
    \---F2
        |   floor_image.png
        |   floor_info.json
        |   geojson_map.json
        |
        \---path_data_files
                5dda52069191710006b573b1.txt
                5de8de3b376b9d0006fdaa5d.txt
```

Each site may have multiple floors, and their floor plans are given along with the trace files (in the folder `path_data_files`). The format of trace files is introduced in `data-format.md`.

In each trace file, there are two parts of data: **metadata** and **fingerprints**. The **metadata** contains the basic information of the collection (e.g., the site ID), and the **fingerprints** refer to the data we collect by smartphones. Please note that due to privacy considerations, we may delete (or change) some sensitive information (e.g., the collector name) in the public dataset. The fingerprints are composed of the following features.

- TYPE_ACCELEROMETER
- TYPE_MAGNETIC_FIELD
- TYPE_GYROSCOPE
- TYPE_ROTATION_VECTOR
- TYPE_MAGNETIC_FIELD_UNCALIBRATED
- TYPE_GYROSCOPE_UNCALIBRATED
- TYPE_ACCELEROMETER_UNCALIBRATED
- TYPE_WIFI
- TYPE_BEACON
- TYPE_WAYPOINT: ground truth location labeled by the surveyor

### Please find the details in `data-format.md`.


