# Mask-Detection

Achieving high accuracy in Mask Detection poses a significant challenge, often requiring a substantial dataset. In this project, we have achieved a 95% accuracy by utilizing a dataset comprising 5708 images. This dataset is evenly split, containing 2854 images with masks and 2854 images without masks.

To attain this level of accuracy, our approach involves the innovative Utilizing MobileSAM, a streamlined variant of the SAM segmentation algorithm, we preprocess the dataset to extract vital insights. This lightweight adaptation addresses the efficiency concerns of the original SAM algorithm, which, due to its extensive computation requirements, can yield results over extended periods. Mobile-Sam offers a more rapid and resource-efficient approach, augmenting the preprocessing phase of our project. Employing Mobile-Sam, we preprocess the dataset, extracting vital insights. The outcome of this segmentation process is meticulously stored within a designated folder.

# MobileSAM

MobileSAM is a refined variant of the SAM segmentation algorithm. Our testing has demonstrated a significant performance improvement: while SAM requires approximately 9 seconds to generate segmented image components, MobileSAM achieves this in just 100 milliseconds.

One of MobileSAM's notable capabilities is the ability to accept input points designated by the user within an image and subsequently return the corresponding segmented region. This functionality is facilitated by harnessing the power of the Mediapipe face detection algorithm, which adeptly identifies facial features and establishes corresponding points.

By incorporating Mediapipe's facemesh functionality, we can accurately pinpoint specific areas within images for segmentation, thus enhancing the precision and customization of the segmentation process.

Through this multi-step process, we not only attain remarkable accuracy but also leverage cutting-edge techniques to enhance our Mask Detection model's performance.
