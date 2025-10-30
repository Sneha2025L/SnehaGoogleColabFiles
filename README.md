Down load files from https://www.kaggle.com/datasets/tysonpo/ice-cream-dataset?resource=download
Refer https://colab.research.google.com/
Refer https://www.kaggle.com/datasets/tysonpo/ice-cream-dataset
About Dataset
🍦 Overview
  1. This dataset contains details (including ingredients), images, and reviews of 241 ice cream flavors across 4 brands (Ben & Jerry's, Häagen-Dazs, Breyers, and Talenti). There are a total of 21,674 reviews, with each review containing star ratings and text. The data was collected directly from the brand websites: (i) https://www.benjerry.com/flavors/ice-cream-pints, (ii) https://www.haagendazs.us/products, (iii) https://www.breyers.com/us/en/products.html, (iv) https://www.talentigelato.com/product-category/talenti-gelato-flavors. Below we describe the three components to this dataset.

products.csv -- Descriptive information about each flavor such as: the flavor name, description, average rating, and ingredients list.
the column key matches the column key in reviews.csv and matches the file name in the images/ directory.
reviews.csv -- Reviews for each flavor. The review information includes: review author, review date, stars (out of 5), review text, upvotes/downvotes (helpful yes/no), etc.
images/ -- The product images.
There are five main directories. Four are for the individual brands: bj/=Ben & Jerry's, hd/=Häagen-Dazs, breyers/=Breyers, talenti/=Talenti. A fifth directory, combined/, contains the merged data. However, since the data reported between the websites is slightly different, there are several NA values in the merged data.

🍦 Uses
There are several uses for this dataset. You could: (i) determine which flavors are most popular, (ii) investigate why popular flavors are popular (e.g. by extracting info from reviews & ingredients), (iii) suggest a new recipe by examining ingredients list, (iv) apply sentiment analysis, (v) compare brands, etc.

🍦 Considerations
The collection of reviews on the brand websites may not be representative of overall opinion, i.e. there may be review censoring or presence of fake reviews meant to help/harm the image of the brand. We intentionally chose brands that host some negative reviews on their website (see e.g. Enlightened or Rebel for only 4-5 star reviews).
Ben & Jerry's, Breyers, and Talenti are all owned by Unilever. Häagen-Dazs is owned by Froneri. Talenti is distinguished from the other brands as they produce gelato.
The images collection probably isn't large enough to use for any computer vision tasks, but may be useful for EDA presentation. Some products may be missing a corresponding image. Ben & Jerry's and Häagen-Dazs images show actual ice cream scoops. Breyers and Talenti only show containers.
Some reviews (mostly specific to Häagen-Dazs) include "…[This review was collected as part of a promotion]" in the text. Also -- not intended -- Talenti's review text seems to also include company feedback, i.e.: "We appreciate your feedback! … please feel free to contact us directly at consumer.services@unilever.com".
🍦 Recent and future updates
In version 1 the data consisted only of Ben & Jerry's and Häagen-Dazs. In the latest version I added Breyers and Talenti data.
I do not have other planned updates, but I may try to add data from other brands (such as Dreyer's). Please let me know if you have any suggestions/questions 😊


In Google Colab use the python script below

# Download latest version
import kagglehub
path = kagglehub.dataset_download("tysonpo/ice-cream-dataset")

print("Path to dataset files:", path)

Based on the output of the dataset download command in cell 8UQh3jeRAZ41, the dataset path is:

/kaggle/input/ice-cream-dataset

# uplod the files to github repository
https://github.com/Sneha2025L/SnehaGoogleColabFiles.git
