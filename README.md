# NonStory – Design

> **NonStory** (a.k.a. "Nonsensical Story") is an improvised party game where players answer given short questions, and as result their answers are composed in a brief nonsensical story which is fun to read!

![NonStory](./Art/NonStory.png)

Here we have specification, art, process diagrams and other design stuff about NonStory.

## Hold a Round

**Round** is considered an interval in which several players participate in game to get a single nonstory out of their own answers. The process of holding it is organized as shown in following diagram:

![Hold a Round](./Processes/Hold%20a%20Round.png)

### Invite Players

![Invite Players](./Processes/Invite%20Players.png)

### Question Players

![Question Players](./Processes/Question%20Players.png)

## Contributing

### Art

We look forward to providing players with better promotional art. Regarding that we ask you to follow some simple rules:
- avoid overloaded graphics with a ton of polygons and curves,
- make sure it follows color scheme provided with logotype and previous promotional art,
- prefer vector graphics when it comes to simpler forms and reusability factor.

### Processes

Making process diagrams in universal form, which is BPMN, is the part of agreeable comprehension.

We use Business Process Model and Notation (BPMN) to describe all possible activities in gameplay and have a perspective look on its extension.

You can use [Camunda Modeler](https://camunda.com/download/modeler/) or other modeler based on bpmn.io to edit or create BPMN diagrams.

What is more, there are rules we use to make more sense of schemes:
- follow [BPMN 2.0 specification](https://www.omg.org/spec/BPMN/2.0/),
- encapsulate hard logic in sub-process,
- apply English title capitalization for activity tasks and sub-processes, also keep them as short as possible,
- if possible, try to associate generic end event with the most ideal outcome (success),
- instead of hoisting same error in scopes of various levels, allocate it a unique signal and handle that in top one (for example look at "Not enough players"),
- specify approximate time for countdown in annotation.
