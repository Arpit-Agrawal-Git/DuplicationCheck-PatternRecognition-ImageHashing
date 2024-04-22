## DuplicationCheck-PatternRecognition-ImageHashing
#### Problem Statement 1: 
Several claims are made annually for product replacement. Images highlighting damage or defect are uploaded with these claims. This is a collection of over 1.5 lakh images in which finding duplicate images (signalling discrepanncy in claims) is like finding needle in a haystack.

#### Solution: 
To address the challenge of identifying duplicate claims among a vast collection of images, we employ an image hashing technique. This method generates a unique hash for each image, which serves as a digital fingerprint. By comparing these hashes, we can efficiently detect duplicate images even within such a large dataset.

#### Problem Statement 2: 
Idenitfy patterns of damage of defect from this vast resource.

#### Solution:
We adjust the hash comparison threshold to cluster images that are not exact duplicates but are sufficiently similar. This allows us to recognize patterns in the defects and damages depicted in the images, providing valuable insights for product improvement.
We also use a variation of this script where we provide a template of defect/damage and check for matching images. This helps gather crucial evidence to cue quality control into corrective or precentive action.
