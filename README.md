The PTV folder is a complete working folder to perform a multiplane calibration.

- The calibration plate has been imaged at 5 positions along the z axis (positions a to e). The aquarium is empty (air, no water).

- There are four cameras.

- The "test" folder contains:

(1) the "cal - *" and "parameters - *" folders obtained after performing a single-plane calibration on each plane, starting from position a to position e ("cal - a" to "cal - a b c d e").
(2) the "man_ori.dat - *" files that contain the pixel coordinates of four manually selected points, for each single-plane calibration ("man_ori.dat - a" to "man_ori.dat - e").

The final calibration folder ("cal") contains: 

(1) The images ("calib_*_cam*.tif") and orientation data ("calib_*_cam*.tif.ori") for each plane and camera.
(2) The corresponding ".addpar", ".fix" and ".crd" files.
(3) The coordinates of the target points ("*_target_plate.txt"). There are 27 x 27 points on the plate (total 729). The first file contains the coordinates of points 1 to 729, the second plane contains the coordinates of points 1001 to 1729 and so on.
(4) The results of the multiplane calibration ("calib_m_cam*.tif.ori").

IMPORTANT: the "orientation.c" file has been edited (see https://github.com/3dptv/3dptv/issues/10). The old file has been renamed as "orientation_Error.c".

