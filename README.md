# U-Net-Implementation
U-Net implementation for body segmentation.

[Unprocessed Original Dataset](https://www.kaggle.com/datasets/bijoyroy/human-segmentation-dataset)

I get the masks from coordinates of polygons and applied data augmentation. Both images and masks are resized to (256,256). Image shape is (256,256,3), mask shape is (256,256,1). Later images are normalized. TFRecord datasets are shuffled and batched with 32.
At the end, I compressed the TFRecord files.
