# Multi-modal_Joint_Image_Restoration

The inputs are signals captured from the same position by different sensors which are called multi-modal.
For example, RGB image (3 channels), infrared (single channel), depth image (single channel) are different images
of different modality. Besides, RGB images taken from the same camera and position but different ambient can
be viewed as multi-modal images. For instance, day and night shot, flash and no flash shots are examples of this 
category.

We developed unsupervised real-time joint image filtering method.

Aim:
Filter a trget image by the guidance of different modality images to improve the target image. We show different 
appliations here. We obtained state-of-the-art results with significantly faster than available methods.

Applications:

Day-night restoration: Night image has no adequate illumination so it misses th details. By using day image we recall the details from day image and combine it with the ambient information of night image. We transfer structural details from day
image to night image.

RGB-Nir restoration: There are two input images one of which is hazy RGB image. The other one is gray level Nir image. Using
the Nir image we dehaze the hazy RGB image.

Structure transferring: We are given two different images. One of them is used as background and the other one foreground. 
We transfer the details of foreground image onto background image by scaling the details. We create different visual effects.

Flash-Noflash deniosing: The inputs are flash and no-flash images. Flash image carry the structural details but deteriorate 
ambient illumination. Noflash image has ambient illumination information but noisy. To denoise noflash image we exploit
flash image and recall the structural details by combining with ambient information of noflash image. The output is 
denoised noflash image.

Flash-Noflash deblurring: The flash image has structural details. Noflash image is blurred. The blurred noflash image is 
deblurred by recalling the details from flash image yet preserving ambient information on noflash image.

