### Resources

- [fast.ai](https://www.fast.ai/) has a range of resources including free online courses covering [deep learning](https://course.fast.ai/), [natural language processing](https://www.fast.ai/2019/07/08/fastai-nlp/), and [ethics](https://ethics.fast.ai/), a [book](https://www.oreilly.com/library/view/deep-learning-for/9781492045519/), and a [discussion forum](https://forums.fast.ai/). These courses have the aim of making deep learning accessible, but do dive into important details. The 'top down' approach to learning in these lessons was inspired by the approach taken in the fastai courses. 

- *The Hundred-Page Machine Learning Book*, Andriy Burkov (2019), provides a concise overview of important topics across both 'traditional' and deep learning based approaches to machine learning.

- There are a range of initiatives related to the use of machine learning in libraries, or with cultural heritage materials. This includes:
    - [ai4lam](https://sites.google.com/view/ai4lam) "an international, participatory community focused on advancing the use of artificial intelligence in, for and by libraries, archives and museums", 
    - *[Machine Learning + Libraries: A Report on the State of the Field](https://blogs.loc.gov/thesignal/2020/07/machine-learning-libraries-a-report-on-the-state-of-the-field/), Ryan Cordell (2020),* a report commissioned by the Library of Congress Labs,
    - Responsible Operations: Data Science, Machine Learning, and AI in Libraries. Padilla, Thomas. 2019. OCLC Research. [https://doi.org/10.25333/xk7z-9g97.]()

- [3Blue1Brown](https://www.youtube.com/c/3blue1brown/about) a Youtube channel by Grant Sanderson covers topics related to machine learning. The channel aims to make the mathematical concepts more easily understood through the use of animations. This may be a particularly useful resource for developing some intuitions about the maths underpinning deep learning and machine learning for those who are less familiar or comfortable with the notation used in some resources.


#### Other Tutorials 

- We plan to extend these lessons further with additional notebook based tutorials on specific techniques and concepts.

- Taylor Arnold and Lauren Tilton have tutorials available on [deep learning and image analyis](https://www.distantviewing.org/tutorial-dl).

#### Suggested Topics for Further Learning

- Ethics and power have only been briefly discussed. Ethical issues related to machine learning is an active area of discussion both inside and outside of academia. Although the issues will be slightly different when working with historical images, ethical considerations do not disappear. 

- It is worth recognising that the deep learning pipeline is only one part of a much longer process. In the case of newspapers, this begins from the publication of the newspaper and its subsequent ingestion to a collection, followed by its potential selection for digitisation. All of these steps will introduce bias into our dataset before we even begin the data preparation steps of the workflow outlined in this lesson. This is further explored by Lee, one of the creators of the Newspaper Navigator Dataset.[^lee]

- Loss and gradient descent: These lessons didn't have space to go into detail about either the specifics of the loss functions used in both of our models, or the details of how model weights are updated based on the loss. Both of these concepts are discussed in many of the resources above. A useful overview can also be found in a [3Blue1Brown](https://www.youtube.com/c/3blue1brown/about) YouTube [video](https://youtu.be/IHZwWFHWa-w)

- Though the layers of a CNN were discussed in this lesson, we didn't fully explore what each of these layers consists of. In particular understanding the 'convolution' part of CNNs will be helpful for more fully understanding how these models work.

- fastai and Pytorch: we only scratched the surface of these libraries in these lessons, it may be particularly useful to look at fastai's [datablock api](https://docs.fast.ai/tutorial.datablock) and [callbacks](https://docs.fast.ai/callback.core). 

#### Tools and Software Libraries

- [LabelStudio](https://labelstud.io/) was used to create the labeled data used in this lesson, and is relatively simple to use for a range of annotation tasks. 
- [Distant Viewing Toolkit](https://github.com/distant-viewing/dvt) is a Python package "designed to facilitate the computational analysis of visual culture"
- [PixPlot](https://github.com/YaleDHLab/pix-plot) is a tool to visualize image collections based on image similarity. 
- [Pandas](https:/pandas.pydata.org/) is often used to help prepare or load data for use in machine learning applications. Some good resources for learning more about pandas include ['Python Data Science Handbook'](https://jakevdp.github.io/PythonDataScienceHandbook/) and ['Python for Data Analysis'](https://wesmckinney.com/pages/book.html)

#### Access to a GPU 

Although it is possible to train deep learning models without a GPU, it will be a much slower experience and may be impractical for working with larger datasets, or bigger images. For a more detailed explanation of why this is, a [response](https://qr.ae/pNCu83) to a question on Quora might be helpful. The majority of deep learning libraries are intended to be run on GPU's made by [Nvidia](https://en.wikipedia.org/wiki/Nvidia). Whilst one option for accessing a GPU is to build or buy a PC with a graphics card, the setup process can be complicated and expensive. Using a cloud platform will usually be a better starting point. 

At the time of publishing this lesson [Google Colab](https://colab.research.google.com/), [Kaggle](https://www.kaggle.com/dansbecker/running-kaggle-kernels-with-a-gpu), and [Paperspace](https://www.paperspace.com/) all provide access a limited amount of free GPU access. These options may change in the future; a good place to get up-to-date information on options for GPU access may be found on the fastai [forums](https://forums.fast.ai/) 
