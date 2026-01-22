# GSoC 2026 Ideas

This year we will focus on these ideas:

- **AI/ML** - Joplin enables users to manage extensive note collections, including personal notes, images, and other documents. We aim to leverage AI and ML technologies to explore and utilise this data in innovative ways.

- **Security** - As users may potentially store a vast amount of private data in Joplin, security and privacy have always been of utmost importance. We aim to explore ways to further enhance security and privacy measures.

- And you are welcome to suggest your own ideas!

## Information for Contributors

These ideas were contributed by our developers and users. They are purposely vague or incomplete - this is because you are expected to research it and develop it to make it your own project.

## List of ideas

### 1. AI-supported search for notes

When your quantity of notes grows you may reach a point where finding notes is difficult. You may know that a specific note is there somewhere but you can't remember any specific keyword that would allow you to find it.

This project is to provide an alternative AI-based search for your notes. Instead of using the existing [seach syntax](https://joplinapp.org/help/apps/search/), the user would express in English what they are looking for. For example:

- It's a note about a meeting with a company from Germany in 2020 or maybe 2019
- I need the list of tasks I wrote for the website redesign
- Look for the note with the poetry lines about the moon
- etc.

**Expected Outcome**: This can be developed as an external application or possibly as part of the core application. This AI based search should supplement the existing search engine. Perhaps both search engine could share the same search box, and one engine or the other would be activated depending on the query. Final outcome should be an AI-based search engine.

**Difficulty Level**: High

**Skills Required**: TypeScript, ML/AL

**Potential Mentors**: Laurent, Marph

**Expected size of project**: 350 hours

### 2. AI-Generated note graphs

As the user uses Joplin, he may accumulate a large number of notes and may find it difficult to know how they related to each others. We could imagine a folder containing many notes for a website project but the user might want to know what is the core idea for this project, what are the less important parts, and how all these ideas are connected to each others.

The goal of this project is to help the user organise his notes and visualise the dependencies between them using a graph.

The AI would analyse all the notes in a notebook or in sub-notebooks, categorise them, and discover how they are connected to each others.

With the above example, a note that shows a global overview of the website could be central. Then there would be a branch for UX, another one for graphics design, and yet another one for programming and technology. Each branch would be developed further with more notes containing more details for that specific topic.

**Expected Outcome**: This can be developed as an external application, a plugin or possibly as part of the core application. The AI would be analyse the notes specified by the user and will create a graph to visualise the relationships between the notes.

**Difficulty Level**: High

**Skills Required**: TypeScript, ML/AL

**Potential Mentors**: Tessus, Malek

**Expected size of project**: 350 hours

### 3. AI-based categorisation

The goal of this project would be to automatically categorise the user's notes. That would mean for example automatically tagging them using AI or creating notebooks and moving the notes to it. Other applications could be to discover notes that are rarely accessed and move them to an "archive" notebook.

**Expected Outcome**: This can be developed as an external application, a plugin or possibly as part of the core application. The AI should analyse the note collection and suggest ways to categorise the notes to the user. If the user agrees, the program should apply the suggested changes. That could mean creating new tags and assigning them to notes, or creating new notebooks.

**Difficulty Level**: High

**Skills Required**: TypeScript, ML/AL, React

**Potential Mentors**: PackElend, Tessus

**Expected size of project**: 350 hours

### 4. Chat with your note collection using AI

Some users have very large knowledge base in Joplin, sometimes built from clipping thousands of pages. This is curated, carefully selected, and thus it would be good to have a way to "interogate" this content. The UI would be very similar to something like ChatGPT, except that the data would be based on the user's note collection.

The user asks a question, the AI answers, and the user can ask more questions to refine the answer.

**Expected Outcome**: This can be developed as an external application or a plugin. The AI should ingest the note collection. Then a UI should be provided to allow the user to ask questions.

**Difficulty Level**: Medium

**Skills Required**: TypeScript, ML/AL, React

**Potential Mentors**: Malek, Tessus

**Expected size of project**: 350 hours

### 5. Automatically label images using AI

Joplin has a strong focus on [accessibility](https://discourse.joplinapp.org/t/project-2-making-joplin-more-accessible-with-wcag-2-compliance/42371). To enhance accessibility, we aim to use AI to automatically scan all images found within the notes and assign a descriptive label to each one. For instance, an image of the Mona Lisa could be labelled as "A portrait of a woman with an enigmatic smile, featuring a soft landscape background and masterful use of sfumato shading".

**Expected Outcome**: This can be developed as an external application or a plugin. The program should scan the note collection then, for each image, it should generate a detailed description of it using AI.

**Difficulty Level**: Medium

**Skills Required**: TypeScript, ML/AL, React

**Potential Mentors**: Laurent, Malek

**Expected size of project**: 175 hours

### 6. Strengthen the security of the plugin ecosystem

We would like to improve the security of Joplin's plugin ecosystem by reviewing plugins' source code. This requires changes to the plugin build and publishing process. See [RFC: Consider changing how we accept third-party plugins](https://github.com/laurent22/joplin/issues/9582) for details.

**Expected Outcome**: Plugins with reviewed source code, ability to build these plugins from source on a trusted server, and a process for reviewing updates and new plugins.

**Difficulty Level**: High

**Skills Required**: TypeScript

**Potential Mentors**: Marph, Malek

**Expected size of project**: 350 hours

### 7. Support for encrypted notes

In general, notes in Joplin are immediately accessible. However the user may want to lock certain sensitive notes behind a password.

**Expected Outcome**: The user can choose to encrypt certain notes and associated resources. When doing so, they would have to enter a password. The note then can only be decrypted using that password.

**Difficulty Level**: Medium

**Skills Required**: TypeScript, Ability to use cryptographic tools and libraries, React for UI

**Potential Mentors**: Tessus, Laurent

**Expected size of project**: 175 hours

### 8. Password strength indicator

Implement a password strength indicator to help users create stronger master passwords. The indicator can visually guide users on how secure their password is when setting or changing it.

**Expected Outcome**: A UI element that displays password strength as the user types. Feedback to the user on how to improve their password strength (e.g., adding numbers, special characters). Integration with an algorithm like zxcvbn to evaluate password strength.

**Difficulty Level**: Easy

**Skills Required**: TypeScript, React (for UI)

**Potential Mentors**: PackElend, Laurent

**Expected size of project**: 90 hours

## More info

- Make sure you read the [Joplin Google Summer of Code Introduction](https://github.com/joplin/gsoc/blob/main/readme.md)
- To build the application, please read [BUILD.md](https://github.com/laurent22/joplin/blob/dev/readme/dev/BUILD.md)
- And before creating a pull request, please read the [pull request guidelines](https://github.com/joplin/gsoc/blob/main/pull_request_guidelines.md)
