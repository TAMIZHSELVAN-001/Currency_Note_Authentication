                                                            Currency Note Authentication
Abstract:This project aims to authenticate currency notes by comparing a test image against a genuine currency note using computer vision techniques. It employs the ORB (Oriented FAST and Rotated BRIEF) feature detection algorithm to identify and match key features between two images. By analyzing the similarity of detected features, the system calculates a match score and makes a simple determination about the authenticity of the test note. This method provides a low-cost, image-based solution to help detect counterfeit currency, especially in regions where traditional authentication tools may not be readily available.

Purpose:The purpose of this project is to provide an affordable, software-based approach to detect counterfeit currency using basic image processing and feature matching. This tool can assist banks, retailers, and the general public in verifying currency authenticity without the need for specialized hardware.
                                                                    
                                                                  Technologies Used:
Python – Main programming language used for development.

OpenCV – Used for image processing, feature detection, and visualization.

NumPy – Used for numerical operations.

Matplotlib – Used for displaying matched keypoints visually.

ORB (Oriented FAST and Rotated BRIEF) – Feature detection algorithm for identifying keypoints and computing descriptors.

Brute Force Matcher (BFMatcher) – For comparing feature descriptors between images.
                                     
                                                                 Existing Method:
Traditional counterfeit detection methods involve:

1.Physical tools like UV lamps, magnetic ink detectors, and watermark verifiers.

2.Specialized machines using infrared and optical scanning.

3.Manual inspection based on known security features (watermarks, security threads, microtext).

These methods, while reliable, are often expensive, inaccessible, or dependent on human accuracy.

                                                                  Proposed Method:
The proposed system uses computer vision to verify the authenticity of currency notes:

1.Extracts keypoints from both a genuine note and a test note using the ORB algorithm.

2.Matches these keypoints using BFMatcher with Hamming distance.

3.Calculates a similarity score based on how many matches fall under a predefined distance threshold.

4.Uses a simple decision rule (e.g., 40% similarity threshold) to classify the note as “Likely Genuine” or “Possibly Fake”.

This approach is portable, cost-effective, and can be implemented using a standard camera or mobile device.

                                                                      Usage:
1.Banking & Retail: Quick on-the-spot verification of currency.

2.Mobile Applications: Can be extended into mobile apps for public use.

3.Educational Tools: Demonstrates practical use of feature detection in real-world scenarios.

4.Prototyping for Security Systems: Serves as a foundation for developing more robust authentication systems.

                                                                      Conclusion:
This project successfully demonstrates the feasibility of using OpenCV and ORB feature matching for currency note authentication. Although it is a basic implementation, it provides a functional and lightweight method for verifying notes with decent accuracy. The approach is ideal for initial filtering and can be enhanced further using machine learning or deep learning for improved performance and robustness against variations like lighting, orientation, and wear-and-tear on notes.
