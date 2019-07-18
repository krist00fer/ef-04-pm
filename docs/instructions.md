# Instructions
## Part 1 - GitHub

You are the one leading a new project forward and need to setup a basic backlog of items to work against so that the rest of the team can 'hit the ground running' once they arrive. You have been given the following background and requirements.

### Background for Part 1

> Background and requirements are meant to simulate real life, but sometimes might make little or no sense. This shouldn't affect the training but is rather a result of poor fantasy by the author, please feel free to make up any missing information yourself.
 
* You are preparing for an upcoming code-with-engagement and the customer have asked us to use GitHub as it conforms to the company policy of the customer that most often do develop in public with an Open Source License (MIT).

* Customer have IoT Devices that already are setup to send telemetry to Azure IoT Hub, but nothing more currently works. We are tasked to build the software that consumes the incoming messages, transforms them to a coma separated text format and eventually stores them on Azure Data Lake. If we achieve this, the customer talks about this as Version 1.0.

* The customer will the continue and build and deploy ML-models for predictive maintenance on top of the data, but that is outside of the scope of our engagement.

> As I mentioned, in real life there would be hundreds of questions that need to be asked in order to correctly setup a correct solution for the customer. At this point, just make up the answer to any question you might have.

### Todo in GitHub

> As mentioned before, the instructions will not be as explicit as before but requires you to find a way forward yourself. This is both due to the hard nature of writing good instructions that will stay relevant when user interfaces changes and also that it's important for you to get a chance to test and try, perhaps much more than just follow exact instructions.

> There are multiple ways to achieve the same thing, you don't need to follow the instruction below strictly.

1. Setup a new GitHub repository, and make it available to the public. Include a README.md file and use the MIT license

2. Use the Tabs in your Repository to go to the Project Tab, create a new project and name the Project board `Ingest Pipeline` and use the `Automated Kanban` template.

> The automated Kanban template isn't necessary, but rather something you and your team should agree upon. Even if you select a specific template you can always change it later.

3. In the `Todo column` you'll see a few `cards` that GitHub adds for you automatically. Review their content since it contains useful information and then `Delete note(s)` using the context menu (the three dots `...` available in the top right corner of all notes).

4. Start adding `To do notes` in the `To do column` by clicking on the plus sign. We'll later convert these notes into full blown issues (GitHub uses Issues to track everything from features and tasks to bugs). Create the following or similar notes:

* Setup skeleton solution to hold source code for ingest pipeline
* Fix access to Azure Subscription for DevTest environment
* Setup CI/CD
* Implement code to consume messages from IoT Hub
* Implement code to transform messages
* Implement code to save transformed messages to Azure Data Lake
* Hand over documents to customer

> Notice that it's quite easy and fast to create a lot of notes this way and it allows you to change your mind, re-order or try things out in a very agile way.

5. When you are happy with the notes you've added we can start converting them to `issues`, the way GitHub tracks all kind of work items and their statuses. Use the context menu on respective notes and select `Convert note to issue`. A new dialog pops up with a possibility for you to write some more context and information.

> Issues in GitHub will later be assigned to a developer to work on, it's important that issues therefor are `small enough` to be fixable by a small amount of developers (often only one) within a short enough time.

6. Your new issues are now automatically assigned to this project. If you click on the issue. You'll see a small popup that shows more information and give you the ability to change some things on this `issue`. Let's go to the issue view instead by clicking on `Issues` in the top menu.

7. The same issues are available here but in a list format instead. Above your issues list, you can see the two options `Labels` and `Milestones`. Clicking on any of them would allow you to create and edit both Labels and Milestones. Labels are used to sort your `issues` into categories while `Milestones` keep track of issues that together will make up a specific achievement (or Milestone) in the project's lifetime. Create a new label called `admin` and a milestone called `v1.0`.

8. Go back to the `issues view` and assign the label `admin` to the issue about fixing access to the Azure Subscription. Assign all but the "hand over issue" to your newly created milestone `v1.0`. Assign a few of the other labels to some "random" issues for you to play around with.

> Notice that issues can have more than one label

9. Play around with the issues list and see how you can filter and sort on the different columns.

10. When the rest of the team arrives, you can use the project board to go through all topics, discuss what you need to do, break down to long issues into smaller new ones, create completely new issues to cover gaps that we didn't think of. Ideally you would do this together with the "product owner".

11. Play around with the project board and move around the issues from `To do` to `In progress` and finally to `Done`. Once everything is in the `Done` column, you are hopefully completely done with Milestone v1.0.

> There are so much more to learn and try in GitHub when it comes to tracking work (issues), but this is the basics and doing this much will lead the team in the right direction.

> What is the first "to-do-item" you could/should put in your backlog? - Create a backlog :-)



## Part 2 - Azure DevOps/Boards


### Background for Part 2

> This time you'll go through the same exercise but this time in Azure DevOps.
 
* You are preparing for an upcoming code-with-engagement and the customer have asked us to use Azure DevOps as it conforms to the company policy of the customer.

* Customer have IoT Devices that already are setup to send telemetry to Azure IoT Hub, but nothing more currently works. We are tasked to build the software that consumes the incoming messages, transforms them to a coma separated text format and eventually stores them on Azure Data Lake. If we achieve this, the customer talks about this as Version 1.0.

* The customer will the continue and build and deploy ML-models for predictive maintenance on top of the data, but that is outside of the scope of our engagement.

### Todo in GitHub

1. Login to Azure DevOps (https://dev.azure.com).

2. In real world we might work in the customers organization and project but this time we'll setup a new organization (name it anything you want) and project. Create a new organization by clicking on the `+ New organization` link in the lower left corner and follow the instructions. If you already have an organization that you feel ok to play around with, you can re-use it instead of creating a new.

3. Inside your new organization create a new project by clicking on `+ Create Project` button in the top right corner. Name your project anything you want, use Private and have a quick look at the options you would have if you click on the `Advanced` options. This is where you can select what "work item process" you want to work with and that will give you different Work Item Types to work with. Keep the default values of `Git` and `Agile`


4. Once created you'll be greeted to your new project and asked how you want to continue. Let's go to `Boards->Backlogs`.

5. This is one of the views where you can create and manage your product backlog. Up in the right corner you should be able to see that we are currently working with `Stories` (User Stories), but you can switch between `Stories` and `Features`. Make sure `Stories` is selected and click on the option to create `+ New Work Item`

> We could have a whole session about how to describe your User Stories and what exact wording to use. Many people use the style: `As a ... I want to ... in order to ...`. Feel free to adopt, change or come up with new user stories that align to this, but for simplicity I've cheated some.

6. Setup the following User Stories

* As a developer, I want to add code to a solution/project that is setup according to standard in order to be effective and collaborative with my team.
* As the build operator and build server, I need access to an Azure Subscription for DevTest in order to deploy new releases manually and automatically.
* As a developer, I need support by a well functional CI/CD pipeline in order to deliver high quality code. 
* As part of the system, we need to consume, transform and save telemetry in order to fulfill the gap that currently exist in the implementation.
* As a catcher of the project, I need documentation that informs me how the system works, in order to quickly be up to date whenever needed.

7. Check out the backlog view and test to re-sort the User Stories by using drag and drop. Then drag the top 3 most important user stories into the `Iteration 1` slot that you find on the right-hand side. This means that we plan to work on these during the first iteration/sprint.

8. Click on the Boards menu item on the left-hand side to see the same backlog as a Kanban board instead. From here you can track and update the user stories as we progress. Try dragging a few of the User Stories to the `Active` column.

9. As you might have noticed the User Stories are a bit more generalized than what might fit a developer to work directly on. During the sprint planning you might decide to break down several or a few of the User Stories into Tasks that are easier to complete and also contains a lot of more detailed and technical information. Click on the `Sprints` menu option in the menu to the left.

10. Explore this view a bit and then make sure you are in the `Taskboard` view. This is a great view for developers to break down User stories into Tasks. Select any user story you want and click on the green plus icon to the right of it and select `Task`. Come up with a few creative task descriptions for a few of the User Stories and try dragging them around on the `Taskboard`.

11. Notice how you can't move a task to state `Resolved` this is since Tasks can't have that state, but bugs can. As you might have seen, you are also able to create `bugs` connected to the User Stories, something that not everyone likes and let's change that for now. Click on the settings icon up on the right-hand side of this view. In the menu go to the section `Working with bugs` and select `Bugs are managed with requirements`. `Save and close` once you are done.

> This change allows us to add bugs in the same views as we are able to add User Stories instead of the one we just worked in.

12. Play around in the different views and explore what you can do and see as the project progresses.

## The End

And we've finally come to the end of this session. Hope fully you've seen that working with both GitHub and Azure DevOps is quite easy and even if we've just scratched on the surface of what can be done, having this much of tools setup for us will give us much value.

I hope you enjoyed,

Thanks, and bye

-Kristofer



