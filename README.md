# InfiniTAM v3

-----

## Build

```sh
cd InfiniTAM/InfiniTAM
mkdir build & cd build
cmake -DWITH_PNG=ON ..
make -j2
```

## Run

* ITM Teddy dataset
  ```sh
  ./Apps/InfiniTAM/InfiniTAM ../Files/Teddy/calib.txt <Teddy-Path>/Teddy/Frames/%04i.ppm <Teddy-Path>/Teddy/Frames/%04i.pgm
  ```

* TUM rgbd_dataset_freiburg1_room dataset (need change image name format `%04i.png` )
  ```sh
  ./Apps/InfiniTAM/InfiniTAM ../Files/TUM/calib_tum1.txt <TUM-fr1-xxx-Path>/rgb/%04i.png <TUM-fr1-xxx-Path>/depth/%04i.png
  ```