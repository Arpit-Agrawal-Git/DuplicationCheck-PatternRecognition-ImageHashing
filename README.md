## DuplicationCheck-PatternRecognition-ImageHashing
#### Problem Statement 1: 
Several claims are made annually for product replacement. Images highlighting damage or defect are uploaded with these claims. This is a collection of over 1.5 lakh images in which finding duplicate images (signalling discrepanncy in claims) is like finding needle in a haystack.

#### Solution: 
To address the challenge of identifying duplicate claims among a vast collection of images, we employ an image hashing technique. This method generates a unique hash for each image, which serves as a digital fingerprint. By comparing these hashes, we can efficiently detect duplicate images even within such a large dataset.

#### Problem Statement 2: 
Idenitfy patterns of damage or defect from this vast resource.

#### Solution:
We adjust the hash comparison threshold to cluster images that are not exact duplicates but are sufficiently similar. This allows us to recognize patterns in the defects and damages depicted in the images, providing valuable insights for product improvement.
We also use a variation of this script where we provide a template of defect/damage and check for matching images. This helps gather crucial evidence to cue quality control into corrective or precentive action.

Image Hashing : A more detailed explaination at https://medium.com/towards-data-science/detection-of-duplicate-images-using-image-hash-functions-4d9c53f04a75

A hash function transforms or maps the input data to a string with a fixed-length which can be seen as the “fingerprint” or “signature” of the input data; the image hash. Thus a good hash function should be fully determined by the input data or in our case, the image. There are various hash functions, such as; Average hash, Perceptual hash, Difference hash, Haar wavelet hash, Daubechies wavelet hash, HSV color hash, and Crop-resistant hash. Each hash function has specific properties to make it robust against certain changes such as brightness, contrast, gamma, correction, watermark, compression, scaling, and grayscaling.

Average Hash Example :

![Average Hash Example](https://github.com/Arpit-Agrawal-Git/DuplicationCheck-PatternRecognition-ImageHashing/assets/88269770/172227cc-cfaa-4238-b3e3-7feb5c79e83a)

Each row in this grid represents a Hash of the image. The first 2 images have identical hash. Next 2 vary at exactly one data point. We can modulate difference threshold to account for such minor difference in near duplicate images.
