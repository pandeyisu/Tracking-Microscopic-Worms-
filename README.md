# Automated software to track microscopic worms *(Heterodera Glycines)* and analyze their behavior in drug environments

This software is written for our [paper] in *Phytopathology*:

Movement and Motion of Soybean Cyst Nematode Heterodera glycines Populations and Individuals in Response to Abamectin
by Jared P. Jensen, Augustine Q. Beeman, Zach L. Njus, Upender Kalwa, Santosh Pandey, and Gregory L. Tylka,
Phytopathology 2018 108:7, 885-891

https://doi.org/10.1094/PHYTO-10-17-0339-R

https://apsjournals.apsnet.org/doi/full/10.1094/PHYTO-10-17-0339-R

Abstract: Two new in vitro methods were developed to analyze plant-parasitic nematode behavior, at the population and the individual organism levels, through time-lapse image analysis. The first method employed a high-resolution flatbed scanner to monitor the movement of a population of nematodes over a 24-h period at 25°C. The second method tracked multiple motion parameters of individual nematodes on a microscopic scale, using a high-speed camera. Changes in movement and motion of second-stage juveniles (J2) of the soybean cyst nematode Heterodera glycines Ichinohe were measured after exposure to a serial dilution of abamectin (0.1 to 100 μg/ml). Movement and motion of H. glycines were significantly reduced as the concentration of abamectin increased. The effective range of abamectin to inhibit movement and motion of H. glycines J2 was between 1.0 and 10 μg/ml. Proof-of-concept experiments for both methods produced one of the first in vitro sensitivity studies of H. glycines to abamectin. The two methods developed allow for higher-throughput analysis of nematode movement and motion and provide objective and data-rich measurements that are difficult to achieve from conventional microscopic laboratory methods.

## Requirments

### Environment Setup

- Download & Install [Matlab R2016a]
- Install Image Processing Toolbox
- Install supported video adaptors for imaging cameras (in our case Q-Imaging)

It was tested on Windows 10 and Mac OS X.

### Usage

- Clone this repo

  ```bash
  git clone https://github.com/ukalwa/track-worms.git
  cd track-worms
  ```

- Open Matlab and navigate to this cloned repo
- To use our video recording software, please run `Matlab/Video/Live_Segmentation.m`
- To segment and generate data of the worm from the video, please run `Matlab/Video/Segmentation/Live_Segmentation.m`
- To analyze the data, please run `Matlab/Analysis/calculate_parameters.m`

## License

This code is GNU GENERAL PUBLIC LICENSED.

## Contributing

If you have any suggestions or identified bugs please feel free to post
them!

  [Matlab]: https://www.mathworks.com/downloads/
  [meanthresh]: https://www.mathworks.com/matlabcentral/fileexchange/41787-meanthresh-local-image-thresholding?focused=3783566&tab=function
  [paper]: https://doi.org/10.1094/PHYTO-10-17-0339-R
