# Architecture Decision Record for Study Planner App
**Decision Title:** Choice of Navigation Strategy
**Date:** Oct 17, 2023
**Team members:** Matthew Yackel, Sergei Mochalov, Steph Martyna, Martin Contreras

## Background
An important decision in the app development process is deciding how the users will navigate between pages. There are several navigation options to consider, including tab navigation (top or bottom), Drawer navigation, stack navigation, tabbed navigation, as well as gestures-based navigation. Our team has researched each method with the goal of determining which navigation method would be most suitable for our app. 

## Decision
After considering the available options, our team has decided to incorporate bottom tab navigation with stack and gesture-based navigation as the primary navigation strategy for our student study planner app.

## Reasoning 
The decision to use bottom tab navigation is based on the following considerations: 
- **Familiarity:** Tab navigation is a widely used navigation strategy for mobile apps and web pages. Using a method that the user is most likely to have used before will eliminate any learning curve for the user. At a glance, the user will be able to understand what the tab nav bar is, and what functions are available in the app. Including gesture-based navigation such as swiping and pinching are also familiar to most mobile users, so we plan to include these inputs to improve user input and app flow within each tab's stack navigation. 
- **Visual Feedback:** With a navigaion bar, the page the user is currently on would be hilighted. This means no matter which page the user is on, they would be able to easily identify where their current location is by looking at the bar. This will reduce the chance that the user gets lost navigating between pages. 
- **Clearly Defined Main Functions:** The navigation bar would include each of the distinct functionalities of the app. The user would be able to see and understand what the main sections of the app are. 
- **Functions Scope:** The navigation bar is ideal for applications that don't have many pages to include in it. Since we plan for our app to have 4 primary pages, a tab navigation bar can cleanly fit and display all 4 buttons. Scalability is also easy to implement if more functionality is added later. 
- **Independent Functions:** Each button on the tab navigation bar will have it's own stack navigation which is independent of the other primary functions. This will maintain a structured and organized way to present content and features. 

## Consequences
While Bottom Tab Navigation provides numerous advantages, there are also potential negative consequences to consider: 
- **Limited Buttons:** While a tab navigation bar is scalable, it is not suited if the number of pages becomes too high. For a navigation strategy that requires five or more buttons, a drawer navigation would be more appropriate. 
- **Screen Size Dependency:** The tab navigation bar is dependent on the height and width of the screen. Mobile devices may have different aspect ratios and resolutions, making the width and sie of the nav bar inconsistent. Accomidations must be considered to keep the navigation bar dynamic to ensure the styling of the buttons remain visually appealing, clear, and functional to the user. The navigation bar is also always displayed on the screen, which takes away screen space from the page content. 

## Conclusion
After in-depth analysis of navigation strategies for our student study planner app, our team has agreed that bottom tab navigation is the most suitable solution. We will also use stack and gesture-based navigation to compliment the naviagtion bar to promote a structured and organized flow. The tab nav bar and gestures will be familiar to users, as well as providing visual feedback to let the user know where they are in the app. With scalability in mind, this strategy will make future functionality additions easy to implement. With careful consideration for device screen sizes and limited amount of buttons available, the bottom tab navigation will enhance the overall usability and user experience of our app. 