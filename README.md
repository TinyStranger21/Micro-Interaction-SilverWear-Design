# Micro-Interaction-SilverWear-Design

Created animated mincrointeractions to add movement and feedback to the checkout process in my SilverWear website.

## Planning

I started by creating sketches showing what the storyboard of the purchasing animations would look like. I started with understanding the general idea of what I wanted. Because this is a website to purchase spoon rings, I wanted all the interactions to be spoon related. I also understood this needed to be catered to the full experience of the purchasing process. What happens when the customer clicks on the ""add to cart"" button and how do we show that the item was added to cart. I mainly worked on providing feedback to the customer after the interactions.

<img width="633.5" height="749" alt="JED   JPP Content Card Sort" src="https://github.com/user-attachments/assets/e525c5b6-8c81-4076-b094-5b7a0937933b" />

# Execution

## Asset Creation

I started by translating my sketches to Adobe Illustraitor in order to get all the assets that I would use in my After Effects animation. After getting what I thought we be used for each key point of the animation, I used Overlord to quickly transfer my vectors to After Effects. This made the process of getting my designs into a animation phase way easier. I kept all vectors in once central area to make sure there was a consisitency with weights and size.

<img width="1080" height="647" alt="image" src="https://github.com/user-attachments/assets/f64aaea5-bb72-4c03-b330-3b318b01d6dd" />

## Animation 1: Spoon to ring to cart

Once I had all my assets exported into After Effects, I started organizing my files and planning what assets were going to move first. I started creating the spoon added to cart animation which shows a spoon swoop into the scene, magically forming into a ring, and then dropping into the cart. There were a few key components that made this animation possible: making the spoon follow a custom path created by the pen tool, custom ease graphs to make the movement feel orgranic and fluid, and collision animations to show the assests in a physicla way.

I watched a good amount of tutorials for this animation because I honestly didn't know how to make some of this movement work, especially the custom path. The custom path was hard because editing the easing graph was very confusing at first and felt like it wasn't working with how I mentally saw this movement. 

One thing I felt really good about with this animation was the stars. Adding this little accent to emphasize a key change in the animation might seem little in the animation but provides a lot of character and flair. This is something I wanted to incoporporate more into future animations.

The last part of this animation came to me after asking severaly people what was off, because it didn't feel complete. At the end of the animation, the cart reacts to the spoon entering with a slight spring animation. This brings a lot empahesis on the final spoon delivery to the cart and provides a sense of closure.

<img width="1728" height="988" alt="image" src="https://github.com/user-attachments/assets/5e4fd628-72b0-43a0-a74e-1e252a0303a2" />

## Animation 2: Add to cart

After I creating the end of the buying experience, I started working on what the initial "add to cart" experience would be like. The core elements of this animation I wanted to achieve were: A seamless text to shape change, a loading experience to provide the customer with a comfortable understanding of the item being added to cart, and final delivery to the cart in the corner animation.

In a book ive read recently, User Friendly by Cliff Kuang and Robert Fabricant, they talk about how some developers and designers purposefully implement loading into products and websites. This creates a sense of trust because it feels like the product is thinking. If the exprience is too quick, its easy to question if the interaction actaully worked. This is a core thing I wanted to add into my animation and I did this through adding a spinning spoon to mimick a classic loading animation.

Once the spoon did its three spins, it exits the "add to cart" button borders and the added to cart animation starts with a very slight delay. I wanted to feel fluid so getting the correct amount of delay that would feel like the spoon that left the "add to cart" was then the spoon that was added to cart. In short, I wanted to make it like one continuous animation.

<img width="1728" height="988" alt="image" src="https://github.com/user-attachments/assets/ca130708-390f-4171-94ca-6eee9e2ba9c8" />

# Implementation

## Figma Layout

Before immediatly implementing the animations into the website, I needed to understand what my purchasing page would look like when the spoon is selected. I followed a pretty standard product layout, pictures of product left, title of product top right, description text below title, "add to cart" below description text. I wanted to make sure the size and weight were most communicated in the purchasing process. I transfered this layout directctly into Cursor in order to get a general idea while also allowing Cursor to accomadate to my current styling in the website.

<img width="1728" height="1117" alt="image" src="https://github.com/user-attachments/assets/7abe1d8e-6d65-4288-ae35-a999ffea7c77" />

## Final web implementation with Cursor

Working with Cursor to implement these animations was, for the most part, not bad. The biggest issues I encountered was placement, sizing, and timing the animations. A lot of CSS is based off left, right, top, bottom, relatives, and offsets, which make it pretty annoying to really get the correct placement for the animtion. One thing I did that made this difficult was I made the actual cart a seperate png than the gif which makes the png look like its animated. This meant I needed the sizing and the placement the exact same in order to make the experience seem seamless.

Once I got this figured out, I moved into adding a number interaction for the cart. Everytime time the "add to cart" button was pushed, the cart spoon animation would play, and once it finished, and red number would intidicate it was added to cart. This number would increase by one everytime the animation would run through a cycle, not immediatly after the "add to cart" button was clicked.

Once I got this function made, I started implementing the "add to cart" loading animation to the "add to cart" button. This animation would play immediatly after clicking, then run one time through. I made the animation a white box that overlays the "add to cart" text so that it can seamlessly add into the button. I needed to create a time delay function that would run the "spoon to ring to cart" animation when the spoon left the "add to cart" box. For this animation process to work everytime the "add to cart button was pressed, I told Cursor it need to reset the gif so that it plays from the beginning everytime, instead of just playing the gif, which would lead to off animation timelimes.

# Conclusion

I think this turned out very well. I am addicted to clicking this button and watching the animation go through. I would say my biggest takeaways from this project mainly came from working with after effects. There are better ways to get a custom motion that just working with the pen tool, and spending way too much time working with eases and trying to the motion in one path, is not worth it.


