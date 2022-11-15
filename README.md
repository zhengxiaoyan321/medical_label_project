# Medical Image Label Project

This readme is used to clarify the problem for this project.

## Project description
### Background
Medical image labeling is hard. Traditionally, accurate labeling are given by domain experts, but the number of experts is very limited, and it's usually costly to consult experts for numerous images. A potential alternative approach to labeling the medical images is to gather the wisdom of the crowd, that is labeling the images by aggregating the opinions of people with less expertise (e.g. students in medical school). The number of non-expert people far exceeds the number of experts, and it usually cost less to get their opinions. Before we can safely accept the labels given by the alternative approach, we would like to know whether the crowd labels the images at least as accurate as the experts.

### Goal
The goal of this project is to show that the crowd labels the images more accurately than individual experts.

### Data Source
The data used in our analysis is gathered by Centaur Labs (https://www.centaurlabs.com/) through their app DiagnosUs. The dataset contains 27000 images, each labeled by 8 experts and several qualified users of the app. The rows of the dataset contains information on: correct label of the image, number of experts who voted on a certain label, number of qualified users who voted on the image, majority vote given by the qualified users, etc. The label given by the crowd is determined by the majority label among all labels by users.

## Analysis and Conclusion
A detailed analysis of the dataset is presented in the Juypter Notebook main.ipynd.

The main conclusion is that:
- When the image is labeled by at least 5 users, the accuracy of the crowd label exceeds the accuracy of the label given by individual experts.
- In general, crowd is more certain with their label than experts.