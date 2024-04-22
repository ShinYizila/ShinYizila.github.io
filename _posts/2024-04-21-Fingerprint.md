# Fingerprint Recognition and System Establishment

Fingerprint recognition is a biometric authentication technology based on the uniqueness of each person's fingerprints. The main steps include **<span style="color:red">collection</span>**, **<span style="color:red">feature extraction</span>**, and **<span style="color:red">matching</span>**. The specific principles are as follows:

1. ![]( https://img.shields.io/badge/Fingerprint%20Image%20Acquisition-8A2BE2)  :Firstly, fingerprint images are collected through sensors. This is typically done using optical sensors, capacitive sensors, or ultrasonic sensors. Fingerprint image acquisition involves having the user place their finger on the sensor.
 <p align="center">
  <img src="https://github.com/ShinYizila/ShinYizila.github.io/raw/master/imageDir/101_1.png" width="200" height="200"/>
 
  
  </p>

2.  ![]( https://img.shields.io/badge/Feature%20Extraction-8A2BE2) The collected fingerprint images are digitized and then undergo feature extraction algorithms to extract key feature points. These feature points may include ridge endings, bifurcations, and ridge lines. The extracted feature points are used to create a unique fingerprint template.
<p align="center">
  <img src="https://github.com/ShinYizila/ShinYizila.github.io/raw/master/imageDir/feature.png" width="200" height="200"/>
</p>

4. ![]( https://img.shields.io/badge/Fingerprint%20Matching-8A2BE2) Once fingerprint features are extracted, the system compares them with registered fingerprint templates stored in a database. The matching process usually involves algorithms to calculate the similarity between two fingerprint templates. If the similarity exceeds a certain threshold, the two are considered a match, thus verifying the user's identity.

5. ![]( https://img.shields.io/badge/Authentication/Identification-8A2BE2)**<span style="color:red">:</span>** Finally, based on the matching result, the system performs the corresponding action. If the match is successful, the system authenticates the user's identity or identifies the user. Otherwise, the user is denied access or needs to undergo additional verification steps.
<div>
<p align="center">
  <img src="https://github.com/ShinYizila/ShinYizila.github.io/raw/master/imageDir/mainframe.bmp" width="300" height="200"/>
  <img src="https://github.com/ShinYizila/ShinYizila.github.io/raw/master/imageDir/similar.png" width="300" height="200"/>
</p>
</div>
Additionally, these methods are encapsulated to establish a fingerprint recognition system. This system can batch add fingerprints and compare fingerprint similarities.

Throughout the process, fingerprint recognition systems rely on the uniqueness and stability of fingerprints. Since each person's fingerprint pattern is unique, fingerprint recognition is widely used in security applications such as unlocking smartphones and access control systems.
