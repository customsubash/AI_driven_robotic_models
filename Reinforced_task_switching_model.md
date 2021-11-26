# SMART Action Model using AI

Looking at the very fundamental operation of human themself, we see that human also do most a task at one time. Thinking about different topics and executing those cannot happen simultaneously which indicates that human do tasks sequentially. A sense of multi-tasking is realized by switching between different tasks. Example if i have to see a movie as well as chat with my friend, at a single instance whether i will be chatting or i will be looking at the movie. I can't do both while chatting as well as watching movie.

Motivated with this model we human also cant deny to have. We can also aspire the robot to implement similar but simple model. Actually similar approach already exists in our computers which runs a task scheduler to run task in its processor fast enough to create a sensation of multitasking.

With robots we will always want them to follow our instruction. Manufacturing factories uses robot to assemble part which they so as instructed with high precision, for this they need the detailed instruction. I think the research should be and is focused on making the robot to do task with very high label instruction (no need to give detailed instruction as to industrial robot) like,

"**GO AND GIVE THIS TO PERSON A"**

Description: 'THIS' may be a object in hands of the user. It should have to grab or detect if the object to be delivered is placed in its compartment. And **A** may be anywhere in the room/scene or may be at a certain distance. The robot would have to search for **A** first and  make an optimal path to reach him. On the way he should not collide with any object or people and finally deliver the object to **A** by also notifying that the delivery is for him.

Now In order to implement the similar model, we will first have to identify the abilities of the robot i.e. the different tasks it can perform.

Current task we can work on

- navigation
- follow dynamic target
- Interact with people/person

And we would like the robot to not only do the given task but also switch to other appropriate tasks on its way. On the basis of scenarios in vision (like when detecting a known person ), robot may interact with them for a while, to control the behavior we can enforce a reward model to give motivation for continuing the task or drop or switch to another one on the basis of:

- Actual command given by the user/master
- Objects in the scene
- Time elapsed in the task
- Task completion percentage
- Goals

We could implement a Reinforced model as we can see we have developed a concept of reward in this model.
