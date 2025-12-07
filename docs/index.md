# Eye-Based Heart Disease Detection Using Machine Learning

Machine learning has become a powerful tool in medical imaging, and this project explores an innovative question: can retinal images be used to predict heart disease? Because the small vessels in the eye often reflect cardiovascular health, the retina provides a unique and non-invasive window into the body. This project examines that connection by developing two predictive models—one deep learning–based and one statistical—to assess how accurately heart disease can be inferred from retinal fundus photographs.

The first model is a Convolutional Neural Network (CNN), built to automatically learn meaningful visual patterns from images. After preprocessing and normalizing the retinal images, the CNN was trained to classify whether each patient had heart disease. A second model, logistic regression, served as a baseline, using extracted grayscale histogram features rather than raw pixel data. Comparing these two approaches helped illustrate the benefits and limitations of deep learning on small medical datasets.

Although the dataset was limited in size, both models offered valuable insights into the visual signatures that may accompany cardiovascular conditions. With further dataset expansion, additional augmentation, or more advanced architectures, the predictive performance could likely improve. This project demonstrates a meaningful step toward using eye-based imaging as an accessible screening tool.

To explore the full analysis, model development process, and code, visit the GitHub repository linked below.

**🔗 GitHub Repository:**  
https://github.com/<katarinatmb>/eye-heart-disease-ml
