# FIGR-8

The FIGR-8 database is a dataset containing __17,375 classes__ of __1,548,256 images__ representing pictograms, ideograms, icons, emoticons or object or conception depictions. Its aim is to set a benchmark for Few-shot Image Generation tasks, albeit not being limited to it. Each image is represented by __192x192__ pixels with grayscale value of 0-255. Classes are not balanced (they do not all contain the same number of elements), but they all do contain at the very least 8 images.

![](figs/dataset_proportion.png)

The main contribution of this dataset to the community is the __abundance of image classes__, which is valuable for tasks in which encompassing an abundance of concepts can be useful or even necessary. This was the case in our paper, [FIGR: Few-shot Image Generation with Reptile](https://arxiv.org/abs/1901.02199 "arxiv link").

The dataset is readily available for people who want to give a shot at few-shot image generation techniques, while spending minimal effort on gathering a full-size database. We also encourage this dataset to enable reproduction efforts from the community.

![](figs/dataset_explanation.png)

### Contents

+ Data/
    + All images are contained in subfolders inside Data folder.
+ data.csv with the following information in order (see below for example):
    + Category number. All items from the same category name have the same category number. One category number per category name.
    + Category name. Also called "class". Represents what is depicted in the image.
    + Path. Represented as Category name/image_id. All images are in 192x192 with .png extension.
	+ Artist. The artist who designed the logo, the icon or the pictogram.
	+ License. The license type which the image is subject to. Refer to section License for more information.

Sample from data.csv:

| Category number  | Category name | Path | Artist | License |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| ... | ... | ... | ... | ... | 
| 11779 | mountain | mountain/1459598-200.png | shastry	| creative commons  |
| 2236| cup| cup/1471583-200.png | simon farkas | creative commons  |
| 11960| plane earth | planet earth/739440-200.png | symbolon |  creative commons  |
|...|...|...|...|...|

### Alternate Download

Alternatively, you can download the dataset from [here](http://bit.ly/FIGR-8 "FIGR-8 GoogleDrive").

### SVG images
If you prefer to work with .SVG images (vector graphics) images, you can download an alternate version of the images from [here](https://drive.google.com/drive/folders/1X3nm_ppvrI1U5YAe5T40ycaRyro-2Gre?usp=sharing "FIGR-8-SVG GoogleDrive").

### License

Most images in the dataset have been licensed under a Creative Commons License by their author, indicating that their reproduction on any material intended to be sold or to be made profit from is **strictly prohibited**. However, use in which the author&apos;s name is indicated is permitted. More details can be found [here](https://creativecommons.org/licenses/by/3.0/us/legalcode "Creative Commons 3.0").

The dataset itself (FIGR-8) is protected under the [MIT License](https://opensource.org/licenses/MIT "MIT License").

### Acknowledgement

Images were gathered from [The Nounji App](https://thenounproject.com/nounji/ "Nounji"), available on the App Store.

If you use this database for your own projects, please consider __citing the following paper__:

	@article{FIGR2019,
	author = {Louis Clouâtre and Marc Demers},
	title = {FIGR: Few-shot Image Generation with Reptile},
	journal = {CoRR},
	volume = {abs/1901.02199},
	year = 2019,
	ee = {http://arxiv.org/abs/1901.02199},
	month = jan,
	archiveprefix = “arXiv”,
	number = “1901.02199v1”,
	eprint = “1901.02199v1”,
	primaryclass = “cs.CV”,
	nonrefereed = “true”
	}
