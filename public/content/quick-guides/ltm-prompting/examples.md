---
title: Use Cases and Example Prompts
path: /quick-guides/ltm-prompting/examples
visibility: PUBLIC
status: PUBLISHED
description: Here are some typical use cases for Pieces Long-Term Memory based on user prompts. This is just a starting point for exploring its capabilities.
metaTitle: Long-Term Memory use cases and example prompts | Pieces Docs
metaDescription: Explore use cases and example prompts for Pieces Long-Term Memory to enhance workflow recall, code assistance, and productivity.
---

## In This Guide

There are many ways to use and prompt LTM to find specific information, recall past fixes and solutions, refresh your memory from conversations and shared resources, and much more.

In this guide, you’ll find some carefully selected use cases and examples that our users commonly rely on—but this is just the beginning.

## Summarize & Extract Information

If you're reading a document in your browser, a PDF viewer, or a collaboration tool like Teams, Pieces is reading along with you. This means you can use Pieces to summarize or extract information from those documents.

Try using these prompts to recall information captured by LTM while you were reading text in a browser or application related to your workflow.

<Steps>
  <Step title="Prompt #1">
    “Summarize the Project Falcon report I was reading last week.”
  </Step>

  <Step title="Prompt #2">
    “I was reading a Red Team huddle report yesterday. What were the items on the agenda and who were they assigned to?”
  </Step>

  <Step title="Prompt #3">
    “Last month I was looking at documentation on the Endor API. What is the API endpoint to open the bunker?”
  </Step>
</Steps>

## Get Deep Link URLs

When Pieces captures context from your browser, it saves the URL you were visiting.

It also captures links from other content where the URL is present in the text, so you can search for URLs, such as finding tabs you no longer have open or retrieving links mentioned in chats or emails.

<Callout type="info">
  Note that Pieces is not a search engine—it captures *memories* from your activities. It will return the URLs you viewed, interacted with, or were shared with you, but it doesn't perform web searches.
</Callout>

Use similar prompts that include a little context, so LTM knows what information to surface and return to the Pieces Copilot.

<Steps>
  <Step title="Prompt #1">
    “Give me the URL of the Yavin JavaScript framework I was reading about this morning.”
  </Step>

  <Step title="Prompt #2">
    “What is the URL for the Power Converter documentation I was reading last week?”
  </Step>

  <Step title="Prompt #3">
    “I need the URL that Leia shared with me with the GCP Firestore database containing the plans.”
  </Step>
</Steps>

## Research an Error in Code

When you encounter an error in your code, whether it's in your terminal, a popup in your IDE, or an error in your browser, Pieces captures it.

* If it's an error you've seen *before*, you can ask about it to recall what you did to fix it.

* If it's a *new* error, you can use Long-Term Memory along with file or folder context to help find a solution in your codebase.

One of the most powerful applications of LTM context and the Pieces Copilot is to facilitate intelligent debugging regarding your recent or active development workflow.

<Steps>
  <Step title="Prompt #1">
    “What was the error I just saw in VS Code? Summarize some of the reasons I may have got this error and give me suggestions to resolve it.”
  </Step>

  <Step title="Prompt #2">
    “I just had an error log in my browser. What was the error and what file did it reference?”
  </Step>

  <Step title="Prompt #3">
    “How can I fix the error I just got in Warp in this project? *(Using the project as a folder of context)”*
  </Step>
</Steps>

## Summarize Recent Work

Knowledge workers often have to provide status updates, such as reports on the work they have been doing or the status of a project.

For example, developers often attend a daily standup where they list the tasks they worked on the previous day and the tasks they plan to work on today.

With access to all your activities, Pieces can help automate this process.

<Callout type="tip">
  Pieces prioritizes activities based on how often workstream activities are captured. This means that documents or applications you spend more time on will be given higher priority in the response.
</Callout>

If Pieces has access to calendar apps, the column or grid format might not be easily understood by AI, which can lead to confusing responses. You might get better results by adding your calendar apps to the list of disabled sources.

Use some of these time-based example prompts to ask Pieces Copilot to provide accurate, relevant answers summarizing recent activities.

<Steps>
  <Step title="Prompt #1">
    “What was I working on yesterday?”
  </Step>

  <Step title="Prompt #2">
    “Give me a list of all the GitHub issues I was looking at yesterday in the Mustafar project.”
  </Step>

  <Step title="Prompt #3">
    “Summarize all the documents I was editing yesterday in Chrome and give me back a list of 5 bullet points that lists my main activities.”
  </Step>
</Steps>

## Get Next Steps

Pieces can detect any upcoming activities, such as tasks in a task management tool, emails in your inbox, or discussions around future work in chat tools.

You can then ask Pieces to summarize these to give you details on what your next priorities are.

<Steps>
  <Step title="Prompt #1">
    “What is next on my agenda?”
  </Step>

  <Step title="Prompt #2">
    “What are the tasks Luke asked me to look at?”
  </Step>

  <Step title="Prompt #3">
    “What tasks are still open in my to-do app?”
  </Step>
</Steps>

## Get Project History

As you work on multiple activities for a project, Pieces is able to piece together memories by capturing relevant context from multiple applications.

This allows you to prompt asking for information about a project and get a response that reasons over all these memories.

<Steps>
  <Step title="Prompt #1">
    “Summarize the carbonite freezing project and give me links to relevant documents.”
  </Step>

  <Step title="Prompt #2">
    “Who are the main contributors to project R2, and what are their email addresses?”
  </Step>

  <Step title="Prompt #3">
    “Give me an overview of the work done so far on D2, and what are the next steps?”
  </Step>
</Steps>

## Get a Summary of Project Status

If you are in a role where you are often receiving project updates and summaries, it can be hard to stay on top of them all.

Pieces can read these updates with you, and provide summaries or roll-ups as needed.

<Steps>
  <Step title="Prompt #1">
    “Give me a summary of all the status updates I received last week from Han, Cassian, and Shin.”
  </Step>

  <Step title="Prompt #2">
    “Write me a summary report on the status of the Phasma testing.”
  </Step>

  <Step title="Prompt #3">
    “Send me a list of all the Jira tickets mentioned in the Geonosis status updates channel in Teams.”
  </Step>
</Steps>

## Summarize Any Text Resource

Sometimes we come across different sources of information that might conflict or vary in detail. This could include anything from news articles to recommendations for code frameworks, cars, and more.

To help make sense of this and get a clearer understanding, Pieces can read all the sources with you, allowing you to think through these memories.

<Steps>
  <Step title="Prompt #1">
    “Summarize the 3 articles I was just reading about the recent stock market trends around AI.
  </Step>

  <Step title="Prompt #2">
    “I was just reading documentation on the best JavaScript framework to use. Provide me a detailed summary containing a list of all the frameworks, their pros and cons, and the maturity of each framework.”
  </Step>

  <Step title="Prompt #3">
    “Based on the reviews of different SUVs I was just looking at in Edge, which one would be the best for a family of 3? I care most about the lowest environmental impact, and the best crash safety.”
  </Step>
</Steps>