![midjourney image](images/midjourney.jpg)

# Using Neural Networks to Detect AI Art

While AI has been used to generate images since its inception, the use of deep learning to generate images resembling art has only recently been brought to the public forefront. Following the public releases of diffusion-based image generation models in mid-2022 such as DALL-E 2, Midjourney, and Stable Diffusion, various moral and ethical concerns have been raised regarding their outputs and methods<sup>[1]</sup>.

<p align="center">
  <img src="images/tweet.png" alt="arin hanson tweet" width=600/>
</p>

One concern is that it will be increasingly difficult to tell human-created art from images generated by models. While humans are often better at classifying objects compared to neural networks, a neural network might be useful in detecting the lower-level nuances that distinguish human art from model-generated images. **In this project, we demonstrate that neural networks can detect whether an image is AI-generated, and that transfer learning is surprisingly (or unsurprisingly) powerful for performing this task accurately.**

## Data

The [dataset](https://www.kaggle.com/datasets/superpotato9/dalle-recognition-dataset) used for this project was found on Kaggle. It consists of ~2,500 each real and generated images. The images were generated by the DALL-E 2 model. The image subjects vary greatly, and include portraits, landscapes, and abstract shapes.

<p align="center">
  <img src="images/data.png" alt="DALLE and real images" width=800/>
</p>

## Methods

In order to observe the effectiveness of various different neural network types, we started training simpler models on the data and progressed towards more complex and powerful models and methods. The data was split into training and test sets randomly and with a 80-20 split.

### Simple Neural Network

The first network trained on the data had a single layer with a RELU connection. The result was 59% accuracy, which was slightly better than random guessing or picking the most common option. 

<p align="center">
  <figure>
    <img src="images/simple_loss.png" alt="simple loss function" width=500>
    <figcaption>Loss function for the simple neural network. It does not show much learning. </figcaption>
  </figure>
</p>

### Convolutional Neural Networks

### Transfer Learning

## Discussion

## References

<sup>[1]</sup> @egoraptor. "Look, you can just say “it’s important to me that a human person made this thing.” All this hogwash about how AI art is ugly… you care about people and that people make art. It’s important to you. You’ve just never had to face that because it’s always been a given until now." *Twitter*, 3 March 2023, 10:07 am, [https://twitter.com/egoraptor/status/1631717867421933583a](https://twitter.com/egoraptor/status/1631717867421933583a).

