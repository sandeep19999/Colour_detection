# Colour_detection

It is the process of detecting the name of any colour.Here,we built an application using which we can automatically get the colour by clicking on it.So,for this we need a dataset consisting of colour name and their rgb values.There are 16.5 million colours which we cannot take in a dataset, so we take only some colours in the dataset and for remaining colours we map them with their nearest colour that is present in our dataset.Dataset is present in colors.csv file which includes 865 colours along with their r,g,b values and hex values.

This project is done using openCV and pandas python libraries.Firstly we require an image to work with.For the working of project we took colorpic.jpg image to find different colours pesent in that image.Using pandas we read the csv dataset to find colours.

User clicks on the image and we have to say the colour present at that position of the image.So, we need to find the x,y co-ordinates on the image where user wants to find the colour. To find the co-ordinates we request a mouse callback event for doubleclick.We calculate the rgb values of the pixel which we double click.When the double click event occurs, we find the rgb values at the position where the mouse double click event occured.

After finding rgb values,we will look for the values in the dataset.If it is present then we print the corresponding color name on the screen.Otherwise we calculate the nearest possible colour that is present in the dataset and print the corresponding colour.
