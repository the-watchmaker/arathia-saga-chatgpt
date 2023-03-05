<img src="https://user-images.githubusercontent.com/4682613/221371974-a81510ce-8b1a-4f1b-9b29-e2e8f6b19ce2.png" width="420" />

The delegates from the kingdoms attending the funeral of the late Arathian Emperor.  [^1]


# The Arathia Saga - Five Kingdoms

_written with ChatGPT_

## How to navigate
- All in markdown at the moment. prompt.md contains main prompts used
- The generated settings are in `/settings` folder. Where it contains results and "connection" prompts.
- The generated contents are in `/story` where you can read a finished story



## The Prompt Design
The prompts are multi-step and grouped by layers.

1. Data Structure Layer: Define how we are setting up references and information structure such as characters, plot, chapter and sections.
2. Setting Layer: Create settings where the story takes place. The setting is created according to the Data Structure Layer.
3. Story Layer: The actual story generated.

Each layers are then oraganized into different ChatGPT sessions and connected using "connection" prompts. This is due to an issue where the ChatGPT accuracy deteriorates in a single session over time. For example, plots can pollute tiny description of a chapter even though you are not supposed to reveal it at that time.


## Milestone
- To create the first iteration of the entire story (500 pages) within an hour.
- To generate all the images for the characters and illustration for all the chapters using DallE2


## Technical Challenges

### 1. ChatGPT's time awareness

To create forshadowing and several events hapenning in parallel require ChatGPT to understand a timeline. A timeline must be coded to be referred by other data such as events. The vast association using a timeline code often creates inconsistency and errors in stories.



### 2. The "connection" prompts create inconsistency between the connected sessions 

The accuracy of the story decreases in a single session with the current version ChatGPT (Mar 2023.) So you need to re-feed the "connection" prompts into a new session. Currently the "connection" prompts" are creating inconsistency between sessions. So, you need to strategically structure each sessions. Top->down structure is a good example. You can create 3 separate sessions: Plots -> chapters -> Parts. This way the details do not get polluted by bigger plots. 




## TODO

### Integration with API

API might yield different result. So it's worth to give a shot. Creating an assisted UI can be an option. Maybe using Next.js to quickly create one?


[^1]: Image generated with DALL-E 2. Prompt for the image: "Five kingdoms fighting over the land of Arathia after the death of the emperor Dashka. Five kingdoms, five armies, five cultures, five landscapes.  The delegates from the kingdoms attending the funeral of the late Emperor. Set in industrial era, in Final Fantasy 5 art style. science fiction. I need a poster without any texts."
