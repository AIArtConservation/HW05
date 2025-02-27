# HW05

I chose the Salesforce "blip-image-captioning-base" model because I wanted to explore how to utilize images to generate text, specifically about what is inside the images. I have been working on a project for another class I’m taking this semester, where I use subway exit signs to generate AR content. So, I wanted to see if I could extract the text from subway signs and trains. However, I also wanted to conduct some generic testing on various kinds of objects beyond just trains and signs, to get a better understanding of what the model performs best on. To do this, I tested it with images of people, cats, and dogs. This helped me become more comfortable with actually using the model and running it. At first, I just used the example code provided on Hugging Face to understand how to use it and then customized it for my test cases.

Here are some things I noticed:

1. Some of the observations for the trains were also pulled from the file name, the date of the photo, and the type of photo (stock or not).
2. However, without prompts, the model makes many assumptions about the trains and often does not even get the city correct, even though all the images are of New York City subway trains. At times, even with prompting, the model gets the city wrong.
3. After trying a lot of different grammar structures and words while prompting, I think it's an iterative process that involves a lot of trial and error to get what I need from the model.
4. Moving on to cats and dogs, the model was quite accurate and was even able to identify the breed of the dogs and cats if they were popular or distinctive enough.
5. I wanted to test what the model had to say about people of various races, so I picked images of actors of the same race for the images I used with the model. I was reading a lot about racial biases and wanted to see what the model would produce.
6. I thought the results it produced were interesting. It seemed to categorize some pictures a certain way and others differently. Namely, in the example where it commented on the skin color of only Black people, but only pointed out similarities in the other picture:
whitemen.webp - The skin color of the people in the picture is the same.
eastasianmen.webp - The skin color of the people in the picture is the same, but the hair color is different.
asian actresses.webp - The skin color of the people in the picture is the most popular.
blackmen.jpg - The skin color of the people in the picture is that of a Black man.
7. Another fascinating thing I found is this: "asian actresses.webp - the skin color of the people in the picture is the most popular." I think this shows how the internet still replicates the prejudices and opinions of real society, and people are still prone to objectification by computers.
8. I also tried extracting text from signs, but I did not get consistent results. However, I would like to explore this further and try out other models to see if I can get better results.
9. I want to look into what factors might be distracting the model from getting out the text on the signs and how I can work around it. 
