# Visual Journal
## iOS Sandbox — Product Overview and Development Plan

### 1. Overview

Visual Journal is an experimental iOS application designed to explore the capabilities of Apple's Foundation Models framework through a personal visual journal.

Users can capture or import photos of objects, places, books, products, and other things they find interesting. The app interprets these images, organizes the information into a personal collection, and allows users to explore their journal through natural language interactions.

The project is intended as a technical sandbox and proof of concept (POC) for an internal company presentation. It is not intended to become a commercial product or be published on the App Store.

The primary goal is to demonstrate how Apple's Foundation Models capabilities can evolve from simple image understanding into a more sophisticated, context-aware assistant.

### 2. Product Vision

Create a personal journal that helps users remember, organize, and rediscover things they encounter in everyday life.

Instead of being just a photo gallery, Visual Journal should help users understand what they have captured, find information within their collection, and discover connections between previously recorded items.

The experience should feel visual, intuitive, and interactive. AI capabilities should be integrated naturally into the product rather than presented as a generic chatbot.

### 3. Goals and Success Criteria

The project should:

- Demonstrate all six selected Foundation Models capabilities through meaningful product features.
- Be developed incrementally, with each stage delivering a functional and demonstrable experience.
- Show a clear progression from basic AI-assisted interactions to more advanced, multi-step experiences.
- Provide a visually engaging interface suitable for a live internal demonstration.
- Make model behavior and output quality observable, allowing meaningful comparisons and experimentation.
- Remain small and focused enough to be developed as an individual project.

Success means demonstrating the capabilities and their practical value, rather than delivering a complete or production-ready application.

### 4. Core User Experience

The application revolves around a personal collection of visual entries.

#### 4.1. Create an Entry

Users can import a photo or select an existing image to create a journal entry.

Each entry should include the image and AI-generated information that helps describe and organize what was captured.

Users should be able to review the generated information and make corrections when necessary.

#### 4.2. Explore the Collection

Users can browse their entries in a visual collection and open individual entries to see their details.

The collection should make it easy to revisit previous discoveries and understand what has already been recorded.

#### 4.3. Search and Ask Questions

Users can ask questions about their collection using natural language.

Example questions include:

- "What books have I photographed?"
- "Find the coffee shop I recorded last month."
- "Which objects in my journal have something in common?"
- "What did I save about this particular place?"

Answers should be grounded in the information available in the journal, rather than relying exclusively on general model knowledge.

#### 4.4. Discover Connections

The app should help users explore relationships between entries and surface potentially interesting connections.

For example, it might identify common themes across several books, connect objects associated with the same place, or help the user explore a topic represented in multiple entries.

These connections should be presented as suggestions that users can explore, not as definitive conclusions.

### 5. Functional Requirements

The application should support the following capabilities across its development stages:

- **Visual input:** Create journal entries from user-provided images.
- **AI-assisted descriptions:** Generate useful descriptions and structured information about each entry.
- **Information extraction:** Identify relevant text and other information present in images.
- **Personal collection:** Store and browse journal entries and their associated information.
- **Collection search:** Retrieve relevant entries based on user queries.
- **Conversational exploration:** Answer questions about the user's collection using its available context.
- **Model experimentation:** Compare the behavior and output quality of different model configurations.
- **Multi-step assistance:** Support more complex tasks that combine information retrieval, analysis, and content generation.
- **Transparent results:** Make it possible to inspect generated descriptions, search results, and assistant responses during demonstrations.

The scope should prioritize a coherent end-to-end experience over the number of features. Each capability should contribute to the central concept of a personal visual journal.

### 6. Incremental Development Plan

Development will be divided into three stages, with two Foundation Models capabilities introduced in each stage.

Each stage should produce a usable increment of the application while establishing a foundation for the next one.

#### Stage 1 — Visual Understanding and Information Retrieval

**Foundation Models capabilities:**
1. Multimodality
2. Integrated Tools

**Objective:** Build the first functional version of Visual Journal, allowing users to create entries from images and retrieve information from their collection.

**Planned functionality:**

- Create entries by importing images.
- Generate descriptions and extract relevant information from each image.
- Organize the generated information into browsable journal entries.
- Search the collection and retrieve relevant information.
- Ask simple questions about previously recorded entries.

**Expected outcome:**

A functional visual journal that demonstrates how AI can interpret user-provided content and combine its capabilities with tools to provide useful, context-aware results.

This stage establishes the core product experience and the data that subsequent stages will use.

#### Stage 2 — Quality Evaluation and Model Flexibility

**Foundation Models capabilities:**
3. Evaluations
4. Model Abstraction

**Objective:** Make the application a practical environment for experimenting with model behavior and evaluating the quality of AI-generated results.

**Planned functionality:**

- Evaluate descriptions and answers against predefined examples and expected results.
- Compare results across different model configurations.
- Identify quality differences, inconsistencies, and potential regressions.
- Separate the application's core experience from its dependence on a particular model implementation.
- Make it possible to experiment with model alternatives without redesigning the user experience.

**Expected outcome:**

A more flexible and measurable application that demonstrates how model experimentation can be incorporated into an iterative development workflow.

This stage should also provide visible material for the internal presentation, showing not only what the AI can do, but how its behavior can be evaluated and improved.

#### Stage 3 — Specialized Assistance and Advanced Reasoning

**Foundation Models capabilities:**
5. Dynamic Profiles
6. Private Cloud Compute

**Objective:** Evolve Visual Journal into a more sophisticated assistant capable of adapting its behavior to different tasks and handling more complex requests.

**Planned functionality:**

- Introduce specialized assistant behaviors for cataloging, researching, and connecting information.
- Select an appropriate behavior according to the user's request.
- Support multi-step tasks that combine collection search, analysis, and response generation.
- Explore how more capable model execution can improve complex tasks.
- Demonstrate how different levels of model capability can complement one another within the same application.

**Expected outcome:**

An advanced demonstration in which Visual Journal behaves less like a simple image-description tool and more like a personal assistant that can investigate and connect information across the user's collection.

### 7. Non-Functional Requirements and Constraints

- **Platform:** iOS.
- **Framework focus:** Apple's Foundation Models.
- **Project type:** Internal sandbox and proof of concept.
- **Distribution:** No App Store release is planned.
- **Scope:** Prioritize demonstrating the six selected capabilities over production completeness.
- **Privacy:** Treat journal content as personal information and make its use by AI features explicit.
- **Reliability:** Handle unavailable capabilities, unsuccessful model responses, and incomplete results gracefully.
- **Demonstrability:** Provide predictable scenarios and sample content that make each stage easy to present.
- **Maintainability:** Keep the application organized so each stage can build on the previous one without unnecessary rework.

The project should not depend on having every advanced capability available during the earliest stages. Development and demonstrations should be designed to accommodate differences in runtime availability.

### 8. Demonstration Strategy

The final internal presentation should tell a progression story through three increasingly capable versions of the same application.

1. **Understand and retrieve:** Show the app interpreting an image, creating an entry, and answering a question about the collection.
2. **Measure and compare:** Show how alternative model configurations behave on the same examples and how their results can be evaluated.
3. **Adapt and reason:** Show the assistant switching between specialized behaviors and completing a more complex task involving multiple entries.

Whenever possible, use the same collection of sample entries throughout all three stages. This will make the progression easy to understand and allow the audience to compare the capabilities directly.

### 9. Out of Scope

The following are not priorities for this POC:

- Commercialization or App Store distribution.
- User accounts, social features, or cloud synchronization.
- A comprehensive production-grade journaling experience.
- Perfect automatic identification of every object or scene.
- Fully autonomous behavior without user oversight.
- Building a complete backend infrastructure solely for the demonstration.

Additional functionality should only be considered when it directly supports the main concept or helps demonstrate one of the six selected capabilities.

### 10. Definition of Done

The project will be considered successful when:

- All three development stages have been completed.
- Each of the six selected Foundation Models capabilities has a clear, demonstrable role in the application.
- The application provides a coherent experience from image ingestion to collection exploration and multi-step assistance.
- Model behavior can be inspected and compared through meaningful examples.
- The final demonstration clearly communicates the progression from basic AI-assisted functionality to more advanced, adaptive behavior.

The central principle is to build one coherent application incrementally, using Visual Journal as a practical environment for exploring the capabilities of Apple's Foundation Models rather than creating six disconnected technical demos.
