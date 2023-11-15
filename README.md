# abstract-art-generation
A DCGAN (Deep Convolution generative Adversarial Network) implementation for abstract art generation. The model is trained on the Art Gallery dataset sourced from Kaggle, providing a diverse range of artistic styles for inspiration.

**INTRODUCTION**
- GAN - Generative Adversarial Network: used in Unsupervised Learning, Generative Modelling
- It consists of two neural networks:
A) Generator: takes random noise and creates
indistinguishable data
B) Discriminator: critic. tries to distinguish
between real and fake data
- 4-step training process:
i) The generator creates fake data from random noise
ii) The discriminator evaluates real and fake data and tries to classify
iii) The discriminator feedback sent to the generator; is used for creating more data
iv) Process repeated iteratively

![image](https://github.com/amithadavid/abstract-art-generation/assets/129505773/42892ba4-287a-4ed5-babc-64bb5e07dc5b)


**METHODOLOGY**
1) Data Collection and Preprocessing
2) Setting up GAN Architecture
3) Training
4) Evaluation and Fine Tuning
5) Generation

**ABOUT THE ART GALLERY DATASET FROM KAGGLE**
- This dataset contains 2782 files of abstract images
- Scrapped from the website: https://www.wikiart.org/
- Use: Content creation, art generation, style transfer, etc.
- kaggle link for dataset: https://www.kaggle.com/datasets/bryanb/abstract-art-gallery/data

**MODEL - DCGAN**
- The goal of this model is to train a DCGAN to generate new works of abstract art.
- The implementation will be done in PyTorch.
- Utilizes the model proposed by the 2015 paper "UNSUPERVISED REPRESENTATION LEARNING WITH DEEP CONVOLUTIONAL GENERATIVE ADVERSARIAL NETWORKS" (which advocates the idea of using stridden convolution to replace pooling layers)

![image](https://github.com/amithadavid/abstract-art-generation/assets/129505773/a343762d-a9ad-4a8e-8055-cb3587920586)


**RESULTS AND DISCUSSION**
- The DCGAN is converging (loss value is stabilizing), which is a good sign.
- GAN is making progress in generating images as the training continues, but not so as exepected. But the discriminator shows amazing progress as the training continues, in detecting which image is fake or real.
- Further training might lead to better image generation quality

![image](https://github.com/amithadavid/abstract-art-generation/assets/129505773/471ede62-5ef5-4d2c-a069-067dc619ed2a)


**CONCLUSION**
- The generated images' visual quality might vary over epochs.
- GAN training often starts with noisy and low-quality images and gradually improves.
- The goal is to achieve visually realistic images as training continues.
- The quality of the generated images can also depend on factors like network architecture, hyperparameters, and the quality of the training data.
- It's essential to evaluate the generated images to assess their quality visually and make further improvements if needed.

**APPLICATIONS**
- Art and Creativity
- Print and Digital Media
- Marketing and Branding
- Video Games and Virtual World
- Art Markets and Collectibles

**EVALUATION**
- Visual inspection
- Diversity of Art
- Quality Metrics
- User Feedback
- Long Term Training
