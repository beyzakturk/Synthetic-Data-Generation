# Synthetic Data Generation

![Image](https://miro.medium.com/max/875/1*R6gx4HIUcIcyCSlQpYWKFA.jpeg)

Synthetic data is artificial data generated with the purpose of preserving privacy, testing systems or creating training data for machine learning algorithms. Synthetic data generation is critical since it is an important factor in the quality of synthetic data; for example synthetic data that can be reverse engineered to identify real data would not be useful in privacy enhancement.

As in most AI related topics, deep learning comes up in synthetic data generation as well. So data created by deep learning algorithms is also being used to improve other deep learning algorithms.

## What is synthetic data?

Synthetic data is artificial data that is created by using different algorithms that mirror the statistical properties of the original data but does not reveal any information regarding real people. For more information on synthetic data, feel free to check our comprehensive synthetic data article.

## Why is synthetic data important for businesses?

Synthetic data is important for businesses due to three reasons: privacy, product testing and training machine learning algorithms. For more detailed information, please check our ultimate guide to synthetic data.

## When to use synthetic data

Businesses face a trade-off between data privacy and data utility while selecting a privacy-enhancing technology. Therefore they need to determine the priorities of their use case before investing. Synthetic data does not contain any personal information, it is a sample data that has a similar distribution with original data. Though the utility of synthetic data can be lower than real data in some cases, there are also cases where synthetic data is almost as valuable as real data. For instance, a team at Deloitte Consulting generated 80% of the training data for a machine learning model by synthesizing data. The resulting model accuracy was similar to a model trained on real data.

## What are the techniques of synthetic data generation?

### Generating according to distribution
For cases where real data does not exist but data analyst has a comprehensive understanding of how dataset distribution would look like, the analyst can generate a random sample of any distribution such as Normal, Exponential, Chi-square, t, lognormal and Uniform. In this technique, the utility of synthetic data varies depending on the analyst’s degree of knowledge about a specific data environment.

### Fitting real data to a known distribution
If there is a real-data, then businesses can generate synthetic data by determining the best fit distributions for given real-data. If businesses want to fit real-data into a known distribution and they know the distribution parameters, businesses can use Monte Carlo method to generate synthetic data.

Though Monte Carlo method can help businesses find the best fit available, the best fit may not have good enough utility for business’ synthetic data needs. For those cases, businesses can consider using machine learning models to fit the distributions. Machine learning models such as decision trees allow businesses to model non-classical distributions that can be multi-modal, which does not contain common characteristics of known distributions. With this machine learning fitted distribution, businesses can generate synthetic data that is highly correlated with original data. However, machine learning models have a risk of overfitting that fail to fit new data or predict future observations reliably.

For cases where only some part of real data exists, businesses can also use hybrid synthetic data generation. In this case, analysts generate one part of the dataset from theoretical distributions and generate other parts based on real data.

### Using deep learning
Deep generative models such as Variational Autoencoder(VAE) and Generative Adversarial Network (GAN) can generate synthetic data.

### Variational Autoencoder
VAE is an unsupervised method where encoder compresses the original dataset into a more compact structure and transmits data to the decoder. Then the decoder generates an output which is a representation of the original dataset. The system is trained by optimizing the correlation between input and output data.

![Image](https://research.aimultiple.com/wp-content/webp-express/webp-images/uploads/2020/07/Variation-encoder-1160x604.png.webp)

## Generative adversarial network
In GAN model, two networks, generator and discriminator, train model iteratively. The generator takes random sample data and generates a synthetic dataset. Discriminator compares synthetically generated data with a real dataset based on conditions that are set before.

![Image](https://research.aimultiple.com/wp-content/webp-express/webp-images/uploads/2020/07/How-GAN-model-works-1160x653.jpg.webp)


