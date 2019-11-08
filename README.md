# Multi-modal_Joint_Image_Restoration

The inputs are signals captured from the same position by different sensors which are called multi-modal.
For example, RGB image (3 channels), infrared (single channel), depth image (single channel) are different images
of different modality. Besides, RGB images taken from the same camera and position but different ambient can
be viewed as multi-modal images. For instance, day and night shot, flash and no flash shots are examples of this 
category.

Aim:
Filter a trget image by the guidance of different modality images to improve the target image. We show different 
appliations here:

Day-night restoration: Night image has no adequate illumination so it misses th details. By using day image we recall the details from day image and combine it with the ambient information of night image. We transfer structural details from day
image to night image.

RGB-Nir restoration: There are two input images one of which is hazy RGB image. The other one is gray level Nir image. Using
the Nir image we dehaze the hazy RGB image.

