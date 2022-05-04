[GANimation model github](https://github.com/albertpumarola/GANimation)
## The code requires a directory containing the following files:
- imgs/: folder with all image
- aus_openface.pkl: dictionary containing the images action units.
- train_ids.csv: file containing the images names to be used to train.
- test_ids.csv: file containing the images names to be used to test.
- To generate the aus_openface.pkl extract each image Action Units with OpenFace and store each output in a csv file the same name as the image. Then run:

- python data/prepare_au_annotations.py
