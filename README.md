## Nutrient Determination and Recommended Meals
This project develops an application that uses the YOLOv8 object detection model and Roboflow APIs[2] to detect food in images and provide a recipe recommendation. The project provides solutions to real-world problems such as food recognition and recipe recommendation using machine learning and artificial intelligence techniques.

The aim of my project is to identify foods using visual object detection techniques and then suggest recipes that are suitable for the identified foods. In this way, users can recognise the foods in an image they have taken or found and find recipes suitable for those foods. For example, when a user uploads an image containing a cucumber, tomato and onion, the programme will recognise these foods and suggest recipes that can be made with these foods, such as salads. This project aims to demonstrate how visual object detection and artificial intelligence technologies can be used in a practical use case scenario.
 
## Training
The model training was done in Google Colab over roboflow using YOLOv8. The training took 2 hours with 1500 photos in total. It is possible to get Api Key[2] by transferring the model to roboflow at the end of the training. In this way, you do not need to download the .pt extension file to your computer and the code is cleaner.[1]

## Data set
I created the dataset myself and labelled it on roboflow. I used 680 photos in total and obtained 1500 photos by data replication.[3]

## Run 
<img src="https://github.com/rumeysakocc/OCT-Diagnostic-Model-and-Interface/assets/115664157/de3ac45d-70ec-4fd7-aa40-825835ab2d40" alt="images" align="left" width="400" height="300">
The project offers a simple and interactive user interface. The interface allows users to select images and get information about detected objects and suggested recipes along with the processed images.

Image Selection: Users can select images through a file explorer or with a file selection button integrated into the interface.

Detected Objects: Objects detected using the YOLOv8 model on the selected image are presented to the user. Each object is shown with the name of the food.

Main Course Suggestion: Main course recipes that match the detected objects are selected from the recipes that pass a certain match percentage threshold and presented to the user. These suggestions provide the user with the main recipes that can be prepared with the specified foods.

Alternative Meal Suggestion: In addition to the main meal suggestions, alternative recipes that do not pass a certain match percentage threshold but can still be associated with the detected objects are also presented. These suggestions allow the user to choose from a wider selection of dishes.

## Database Usage
The project does not extract suggested recipes from a specific database. Instead, using a dictionary of predefined recipes, it finds recipes that match the detected nutrients. This approach ensures database independence and provides users with a variety of meal recommendations.

## Installation and Operation
After downloading the project to your computer, you should make sure that the necessary packages and libraries are installed. Then, you can run the project and process the images using the user-friendly interface.

## References 
[1] ttps://colab.research.google.com/drive/1ipqwlyYj4XftfP6SJDIwYmelodHEhYu?usp=sharing


[2] https://docs.roboflow.com/deploy/hosted-api/object-detection


[3] https://app.roboflow.com/test-wrdoj/food-nkiop/browse?queryText=&pageSize=50&startingIndex=0&browseQuery=true





