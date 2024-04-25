# voyage-project-tier1-color-explorer

## Table of Contents

* [Overview](#overview)
* [General Instructions](#general-instructions)
* [Requirements & Specifications](#requirements-specifications)
* [Acknowledgements](#acknowledgements)
* [About Chingu](#about-chingu)

## Overview

Hello Chingus!

Let's consider the importance of colors in our lives. These bright shades not only decorate our surroundings but also affect our feelings and thoughts every day. From the calming effect of gentle blues to the energizing power of vibrant greens, colors impact how we experience and express ourselves. However, many of us find ourselves struggling to find matching colors, whether for our outfits or interior design, often leading to frustration and uncertainty in our choices.

During this voyage, you will be building a color matching app. The app is intended to serve as a personal consultant, helping users find harmonious color combinations for various purposes, including outfit coordination, interior design, website design, graphic design projects, and more.

- Color theory example site

![Color theory example site](./assets/colorwheel2.png)

- Color theory example site

![Color theory example site](./assets/colowheel1.png)

This voyage takes an even more thrilling turn as Chingu introduces the integration of the OpenAI API for the first time. With this powerful tool at your disposal, you'll craft an innovative solution enabling users to uncover their ideal color combinations.

So, grab your color wheels and dive into coding!

## General Instructions

This project is designed to be worked on by a team rather than an individual
Chingu. This means you and your team will need to thoroughly read and
understand the requirements and specifications below, **_and_** define and
manage your project following the _Agile Methodology_ defined in the
[Voyage Handbook](https://github.com/chingu-voyages/Handbook/blob/main/docs/guides/voyage/voyage.md#voyage-guide).

As you create this project make sure it meets all of the requirements, but once
it reaches MVP, start implementing the optional features or get creative and
extend it in ways we haven't envisioned. In other words, use the power of
teamwork to make it distinctive and unique.

Take note that we haven't given specific direction on what your UI/UX should
look like. This is another area where you and your team can put your creativity 
to work! 

## Requirements & Specifications

### What You Need to Do

The following define the minimum requirements and ideas for features you may
implement to enhance this app, if time permits.

#### Structure

- [ ] This is a purely frontend application. No backend is required.
- [ ] You may use any languages, tools, or libraries you prefer when designing and building this app.
- [ ] You may **_NOT_** use AI-base solution generators like GitHub CoPilot.
- [ ] The app should facilitate connectivity to the OpenAI API for color recognition.
- [ ] Useful links and resources:
  - [Wiki about Color Scheme](https://en.wikipedia.org/wiki/Color_scheme)
  - [OpenAI API docs](https://platform.openai.com/docs/introduction)
  - [Color picker library](https://iro.js.org/)
  - Video Tutorials:
    - [How to Create Color Picker in Javascript & HTML](https://www.youtube.com/watch?v=eIw-Nou9L9E)
    - [HTML | CSS Color Picker ](https://www.youtube.com/watch?v=m-z3xQL9rzU)

  - **API Call Guide** For performing API calls, you can refer to this [example sandbox](https://codesandbox.io/p/devbox/exciting-rain-h5tnmj?file=%2Fsrc%2Findex.html%3A3%2C7). The example demonstrates how to make API calls using JavaScript fetch() method.

  - **API Tutorial Resources:**

    - [Web Streams Tutorial](https://umaar.com/dev-tips/269-web-streams-openai/): This tutorial includes a blog post and a video.
    - [Using Fetch API - MDN Documentation](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch): Detailed documentation from MDN.
    - [Fetch API Tutorial - YouTube](https://www.youtube.com/watch?v=cuEtnrL9-H0): An explanation about Fetch API on YouTube.

#### Styling

- [ ] Surprise us!!! Use your teams creativity to make this app distinctive.
- [ ] Add a footer containing a link to your teams GitHub repo.
- [ ] In general, you will find these [UI design principles](https://www.justinmind.com/ui-design/principles) helpful.
- [ ] Recommend using this resource for [clean CSS](https://israelmitolu.hashnode.dev/writing-cleaner-css-using-bem-methodology).

#### Functionality

-   Overview:
    - [ ] Develop a single-page application (SPA) or its equivalent to deliver intuitive color recommendation functionality to users.

- Color Capture and Processing
    - [ ] Implement a color palette selector allowing users to choose colors from a predefined set.
    - [ ] Provide a minimum of 9 color options represented as boxes on the page.
          
    **Note:** You have the flexibility to implement the identification of each color in a way that suits your design. Consider utilizing unique identifiers for each color box to facilitate interaction. For instance, you might use the color's HEX code or any other method you find suitable. This allows for customization while ensuring clarity in color selection.

- API Connectivity and Response Handling
    - [ ] Establish connectivity to the OpenAI API for color analysis via provided API key.
    - [ ] Send the captured color data to the API as part of the prompt.
    - [ ] When sending color data to the OpenAI API, include it in the prompt along with a request for color recommendations. Ensure it also requests color codes with their respective names for the recommended colors. Example prompt:
      - "Suggest color recommendations based on the [selected color]"
      - "Color recs [selected color]"
    - [ ] Retrieve and process the response from the OpenAI API.
    - [ ] Capture the color codes and text description provided by the OpenAI API in the response.

- Visual Representation
    - [ ] Visualize the response from the OpenAI API using colors and accompanying text.
    - [ ] Represent the AI-generated color response in a visually comprehensible manner within the application interface.

- User Experience
    - [ ] Ensure the application provides a seamless user experience for color selection, processing, and response visualization.
    - [ ] Implement intuitive UI/UX elements to guide users through the color capture and analysis process.

- Responsiveness
    - [ ] Ensure the web application is responsive and accessible across various devices and screen sizes.
    - [ ] Utilize responsive design techniques to adapt to different viewport sizes.

### Extras (Not Required)

- Color Capture and Processing
    - [ ] Create boxes of minimum 9 colors with their HEX code OR Use a color picker library to select color, eg [Iro JS](https://iro.js.org/).
    - [ ] Utilize a library for visually representing color recommendation responses.

- API Connectivity and Response Handling
    - [ ] Ensure robust error handling for API connectivity, data formatting, and response processing.

## Acceptance Criteria

- Color Capture and Processing
    - [ ] Users should be able to accurately select colors using a custom color palette selector.
    - [ ] Captured color codes must be correctly formatted and included in the prompt sent to the OpenAI API for analysis. The prompt should explicitly request color recommendations based on the selected color and ask for color codes to be included in the response from the AI.
    - [ ] The application should effectively process the response from the OpenAI API, providing meaningful insights into the selected color.

- API Connectivity and Response Handling
    - [ ] The application must establish reliable connectivity to the OpenAI API for color analysis.
    - [ ] Response handling mechanisms should accurately interpret and extract relevant information from the API response.
    - [ ] Error handling must be implemented to gracefully manage any issues encountered during API communication.

- Visual Representation
    - [ ] The AI-generated color response should be visually represented in a clear and understandable manner within the application interface, effectively conveying the characteristics and attributes of the analyzed color along with their corresponding text descriptions.

## How to Obtain OpenAI API Key

  - Create an Account
    - [ ] Visit the [OpenAI API website](https://platform.openai.com) and create an account.
  - Navigate to API Keys
    - [ ] Once logged in, go to the API keys section in the navigation menu.
  - Generate a New Secret Key
    - [ ] Click on "Create New Secret Key" to generate your API key.
  - Note for Existing Users
    - [ ] If you are logged in with a ChatGPT account, you won't have access to a free OpenAI API key. Free keys are available for new users and are valid for three months.

## Acknowledgements

We express gratitude to the [OpenAI](https://openai.com) team for providing access to their API, enabling us to incorporate advanced color analysis capabilities into our application.
Additionally, we appreciate the contributions of the wider developer community whose insights and expertise continually enrich our projects.

## About Chingu

If you aren’t yet a member of Chingu we invite you to join us. We help our
members transform what they’ve learned in courses & tutorials into the
practical experience employers need and want.
