# How to make Custom Loss Function in Keras.

This is a tutorial on how to create your own loss function in Keras.

In CustomLoss.ipynb, mainly `Function type` and `Class type` are explained to make custom loss.

There Loss function are inplemented in CustomLoss.ipynb.
- Image MSE Loss
- Image L1 Loss
- Image L2 Loss
- Reconstruction Loss
- VGG Loss
- Gram matrix
- Style Loss
- Multi Style Loss

In Pytorch, you can easily build a loss function by default, but in keras, you need more work. Also, there are surprisingly few web pages on how to create your own functions in keras. However many people use Keras for research or work because it is easy to write. So, we would like to share some tips on how to make your own functions in Keras.

I hope this is useful for you.😎


---
#### References on Loss Function
- [Building Autoencoders in Keras](https://blog.keras.io/building-autoencoders-in-keras.html)
- [Shape preserving loss](https://github.com/ZengqiangYan/Shape-preservingLoss/blob/master/Loss.py)
- [Texture GAN](https://github.com/janesjanes/Pytorch-TextureGAN)
- [Style Loss](https://blog.shikoan.com/style-loss/)

#### References on Inplementation of Loss Function
- [tf.Keras Backend](https://www.tensorflow.org/api_docs/python/tf/keras/backend?hl=ja)
- [TensorFlow, KerasでVGG16などの学習済みモデルを利用](https://note.nkmk.me/python-tensorflow-keras-applications-pretrained-models/)
- [Extract Features, Visualize Filters and Feature Maps in VGG16 and VGG19 CNN Models](https://towardsdatascience.com/extract-features-visualize-filters-and-feature-maps-in-vgg16-and-vgg19-cnn-models-d2da6333edd0)
- [Loss Function Classの作成例](https://memo.sugyan.com/entry/2020/02/16/220750)
- [kerasで自作損失関数を実装したい](https://teratail.com/questions/185516)
- [Kerasで損失関数に複数の変数を渡す方法](https://blog.shikoan.com/keras-loss-function-multiple-arguments/)  
→ Custom Loss function usually receive only (y_true and y_pred).  
→ Q. When you get loss function to get other paramerters.  
→ A. Let's wrap the loss function with another function.



\# Kerasでの自作損失関数の作成方法
