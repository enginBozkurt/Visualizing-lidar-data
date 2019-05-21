# Visualizing lidar data 

Visualizing lidar data using Uber  Autonomous Visualization System (AVS) and a Jupyter  Notebook Application

This project contains two different applications for visualizing lidar data using  KITTI Vision Benchmark Suite datasets.


![ubPic](https://user-images.githubusercontent.com/30608533/58125546-7924eb00-7c19-11e9-93e1-c69c5465edb9.png)




## 1.  Uber AVS Autonomous Visualization System (AVS) ---  XVIZ (the data layer for AVS)

###  Quick start

You need [Node.js](https://nodejs.org/en/) and [yarn](https://yarnpkg.com/lang/en/docs/install) to
run the examples.

```bash
# Clone XVIZ
$ git clone https://github.com/uber/xviz.git
$ cd xviz

# Install dependencies
$ yarn bootstrap
```

Convert and serve KITTI example data:

```bash
# Download KITTI data
$ ./scripts/download-kitti-data.sh

# Convert KITTI data if necessary and run the XVIZ Server and Client
$ ./scripts/run-kitti-example.sh
```


# 2. KITTI Dataset Exploration 

## Dependencies

Apart from the common dependencies like `numpy` and `matplotlib` notebook requires [`pykitti`](https://github.com/utiasSTARS/pykitti). You can install `pykitti` via pip using:

```
pip install pykitti
```

## Project structure

| File                   | Description                                                                                      |
| ---------------------- | ------------------------------------------------------------------------------------------------ |
| `kitti-dataset.ipynb`  | Jupyter Notebook with dataset visualisation routines and output.                                 |
| `parseTrackletXML.py`  | Methods for parsing tracklets (e.g. dataset labels), originally created by Christian Herdtweck.  |
| `utilities.py`         | Convenient logging routines.


I have used one of the raw datasets available on [KITTI website](http://www.cvlibs.net/datasets/kitti/raw_data.php).


2011_09_26_drive_0005 (0.6 GB) 

**Length**: 160 frames (00:16 minutes)

**Image resolution**: 1392 x 512 pixels

**Labels**: 9 Cars, 3 Vans, 0 Trucks, 2 Pedestrians, 0 Sitters, 1 Cyclists, 0 Trams, 0 Misc


![notebook1](https://user-images.githubusercontent.com/30608533/58126353-75926380-7c1b-11e9-9be2-3b2e5177887e.jpg)


![5ce4618251634176609181](https://user-images.githubusercontent.com/30608533/58129044-96f64e00-7c21-11e9-9f7e-7a9b18930ff9.gif)



