# Mosaic-Image
Generate Mosaic Image using [VisualGenome Dataset](http://visualgenome.org/)

Requirements: PIL, Numpy, Pandas, CV2

First, the database of Average RGB need to be created using this script. Then run this script to generate the mosaic images. There are several parameters need to be tuned when generating the mosaic images:

1) pixel_batch_size: control the detail of picture, lower means more detail but takes longer time to produce. 
2) rmse_threshold: control the color similarity, try as lower as possible in the beginning, if there is an error indicating "too lower threshold" then try to add the value slowly
3) allow_use_same_image: if true then the generator is allowed to use same picture many times
4) target_PATH: PATH of the target image
5) DB_PATH: PATH of the Average RGB database created using this script
6) OUTPUT_PATH: destination PATH of the mosaic image output