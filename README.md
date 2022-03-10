# [Research on Generative adversarial networks for Super Resolution](https://github.com/dang3tion/Colab-Super_resolution)
Referenced papers:
:bookmark_tabs:
* [Photo-Realistic Single Image Super-Resolution Using a Generative Adversarial Network](https://arxiv.org/abs/1609.04802)
* [ESRGAN: Enhanced Super-Resolution Generative Adversarial Networks](https://arxiv.org/abs/1809.00219)
* [Generative Adversarial Network for Image
Super-Resolution Combining Texture Loss](https://pdfs.semanticscholar.org/f35f/c5b6237c21f36fc3f00c45dba070e8242c23.pdf)
* [And some related papers](https://github.com/dang3tion/Super-Resolution-Documentary/tree/main/Necessary%20Document)

Environment and platform :computer:
* [Tensorflow 2.7](https://www.tensorflow.org/)
* [Google Colab](https://colab.research.google.com/)

The project is implemented on *Google driver*.
****
# Result
<div align="center"><img src="https://user-images.githubusercontent.com/65795540/157159117-746ec97e-1c8f-46a5-af08-fd75b7384400.png" /></div>
<div align="center"><img src="https://user-images.githubusercontent.com/65795540/157159241-47a06427-971c-4941-9878-4486312222d6.png" /></div>
<div align="center"><img src="https://user-images.githubusercontent.com/65795540/157159279-5437da3b-275a-4f48-9fe1-12203d494fad.png" /></div>

# Implementation
## Architecture:
* Generator ![Generator_architecture drawio (3)](https://user-images.githubusercontent.com/65795540/157160094-052d634d-8cd3-4bce-9fa9-dbd78326452c.png)
****
* Discriminator ![Untitled Diagram drawio (19)](https://user-images.githubusercontent.com/65795540/157160143-6120ab37-76ed-4d26-ac65-5147e0eb1cc9.png)
## Losses:
I implemented 3 loss terms to support Generator reconstruct Super Resolution image:
* Pixel-wise Loss <div align="center"><img src="https://user-images.githubusercontent.com/65795540/157160693-91454525-5ada-43d0-ad14-5d614952ba4f.png" /></div>
* Feature Loss <div align="center"><img src="https://user-images.githubusercontent.com/65795540/157160736-6d120d19-74be-420e-8d49-9c439bff8aab.png" /></div>
* Style Loss <div align="center"><img src="https://user-images.githubusercontent.com/65795540/157160776-d33d4261-059f-46cf-a996-4d28eb855796.png" /></div>
****

And with Adversarial Loss I used LSGAN combine with Relativistic average GAN:
* For Generator <div align="center"><img src="https://user-images.githubusercontent.com/65795540/157160928-24f85c65-2821-47d1-ac63-988d9e3df9c7.png" /></div>
* For Discriminator <div align="center"><img src="https://user-images.githubusercontent.com/65795540/157160963-bab6474a-ab60-4c5f-9bb9-6c927b020963.png" /></div>
## Training
<div align="center"><img src="https://user-images.githubusercontent.com/65795540/157162499-7cd8ee32-b6cb-4403-ae7e-cc478979feba.png" /></div>






