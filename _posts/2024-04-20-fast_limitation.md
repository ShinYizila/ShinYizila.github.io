# Fastai Limitations
## ![Image text](https://img.shields.io/badge/Limitations-grey?style=for-the-badge&logo=javascript)

- **Excessive Encapsulation:** Fastai suffers from excessive encapsulation, making it difficult for users to directly modify the model. For example, extracting features from a specific layer can be challenging.

- **Insufficient Documentation:** The documentation provided by Fastai lacks basic information. Users may find it challenging to perform simple tasks such as modifying batch size as it's not clearly documented in the official documentation or code.

- **GPU Memory Management:** When using GPU, Fastai's memory cleanup is not always thorough, leading to memory fragmentation and affecting subsequent processing speed.

## ![Image text](https://img.shields.io/badge/My%20Own%20Think-grey?style=for-the-badge&logo=javascript)

In training, when the batch size is set to 64, the computation time on CPU for 10 epochs is 357ms. However, when using GPU, the computation time reduces significantly to 34ms, which is approximately 10 times faster than CPU. This difference is clearly evident.

 <div align="center">
  <img src="https://github.com/ShinYizila/ShinYizila.github.io/raw/new/imageDir/cpu64.bmp" width="200" height="100"/>
  <p>cpu time for batch=64</p>
  </div>
   <div align="center">
  <img src="https://github.com/ShinYizila/ShinYizila.github.io/raw/new/imageDir/gpu64.bmp" width="200" height="100"/>
  <p>gpu time for batch=64</p>
  </div>
   <div align="center">
  <img src="https://github.com/ShinYizila/ShinYizila.github.io/raw/new/imageDir/gpu256.bmp" width="200" height="100"/>
  <p>gpu time for batch=256</p>
  </div>
  
When the batch size is increased to 128, the GPU computation time increases slightly to 49ms. Surprisingly, when the batch size is further increased to 256, the GPU computation time increases to 85ms. This observation indicates that as the batch size increases, the computation time does not continue to decrease but rather reaches a minimum and then starts increasing again. This behavior is different from other frameworks such as ![Pytorch]( https://img.shields.io/badge/Pytorch-8A2BE2), which may raise out-of-memory errors when the batch size becomes too large.

Hence, it can be inferred that ![FastAi]( https://img.shields.io/badge/FastAi-fedcba) likely optimizes batch size internally, ensuring efficient computation without exhausting resources.