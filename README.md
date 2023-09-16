

## Inspiration
We were inspired, like all great products in life, by the challenges that people face all around us. Almost everybody deals with some serious health issue in their life, and all of us have as well. And one of the most common medical solutions is prescription pills, which can be hard to differentiate and identify even with 20-20 vision. In fact, we ourselves struggled to find the difference between some well-known medications. If we had the trouble, that would mean those of us who are more vulnerable due to conditions such as bad eyesight or weak hands would have even more difficulty identifying the proper medication. We began researching solutions to this problem and found that most existing platforms use only descriptions of pills to identify the type of medicine, which is not always the most accurate solution. Thus, inspired by this, we came up with a pill identification software, as pharmaceutical companies often make pills very similar and without easily distinguishable markings (made even more difficult if you have bad vision or are floating around in space!). We all wanted to learn more about using ML frameworks and get more hands-on experience using them. So we developed a machine learning model to identify pills based on their images, which would also give us the framework to expand on this project in the future. We wanted to make sure this was easily accessible to potential users, so the model was integrated into an app and through this, MediScan was born!

## What it does
When you open the app, it prompts you to either upload an image or take one of the pills you are trying to identify. From there, it will crop automatically to the optimum ratio and then it will identify the pill within the image. 

As a pro tip, zooming in helps with identification since the camera can see the fine details and make out the grooves that distinguish even the most similar-looking pills!

## How we built it
This app was built using XCode and Swift, and the model was created and trained using CreateML to ensure the model was in a CoreML model format and compatible with iOS app development. The dataset was from Kaggle - credited below! 

## Challenges we ran into
One of the biggest challenges we ran into was finding a comprehensive dataset that had accurate labeling. In the pharmaceutical world, pills have multiple names and features that depend on the company, and the dataset size required would be far too large to be feasible within the time set. While looking over possibilities, we found multiple that were not labeled which would require manpower to go through and divide them up. Thus, we settled on a smaller dataset for a limited amount of pills (10 common medications found within South East Asia), with the framework to expand further with more classification! Thus, in the future (while we're not in as much of a time crunch), we can add more support for pills and even distinguish between brand medications. 

In addition, if we used larger data sets, our training time for our model would take exponentially longer, which was something we were concerned about during our short time :)

One other thing we had to keep in mind is that previous research into using image classification models for pills has yielded relatively imprecise measures. The highest identification percentage we could find was around 70%, and that was within papers published in respected journals such as IEEE. Thus, we had to lower our expectations of what we considered a successful model to be, especially within the given time constraints. We were able to improve slightly on industry standards with our testing accuracy being 72%!

## Accomplishments that we're proud of
Overall, the learning curve of this project was fairly steep, so we are all proud of how much we were able to do! 

We are proud to have created a model that improved on the industry level standard for pill identification accuracy. We are also proud to have made this more accessible for users by including minimal, and easy to use functions. As we mentioned this app is targeted to help those more vulnerable with conditions such as bad eyesight or weak hands. So, we included features such as larger text and minimal interaction requirements to utilize the app. Rather than having users work through a complex amount of instructions or fields to fill out, they simply have to tap with 1 or 2 fingers to take or upload a picture respectively. 

We are also proud to have learned how to integrate a machine learning model into a user-friendly app to make our research more accessible and useful.

## What we learned
All of us had very little, if any, IOS app development experience, so everybody within our team became much more comfortable with developing. Specifically, we learned about implementing our vision in Swift and XCode as well as integrating our ML model into our app. We got more practice with design principles as well since we wanted to work on the design of the app while we were waiting for our model to learn.

On the backend side, we were able to dive more deeply into the back-end details of actually creating our model. We worked to find the optimum split of training and testing data to get the results we wanted from our model, and we also learned the importance of patience regarding training. None of us had ever used CreateML for machine learning and iOS compatibility either, so this allowed us to add another training tool to our skills.

## What's next for MediScan - Pill Identification
Our next steps are to expand our dataset to include more varying types of drugs - specifically, we will target the drugs that are used by vulnerable populations. In addition, without time constraints, we will be able to train our model through further iterations of larger amounts of testing data, leading to a better model. 

## Credits
Dataset - https://www.kaggle.com/datasets/vencerlanz09/pharmaceutical-drugs-and-vitamins-synthetic-images



