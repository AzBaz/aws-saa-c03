
[[0. AWS-SAA-Training Overview]]

# AWS Certified Solutions Architect Associate (SAA-C03) Study Notes

A personal collection of study notes, preparation strategies, and resources compiled while preparing for and passing the AWS Certified Solutions Architect Associate (SAA-C03) examination.

## Overview

This repository contains the notes I recorded in Obsidian during my certification preparation, along with the exam tips and resources that proved most useful. The material is organized by AWS service domain and reflects my own study methodology.

Please note that these notes are subjective and may not align with your preferred approach to studying. You are welcome to adapt or edit them to suit your own needs.

Repository contents:

- Forty-nine topic notes covering the SAA-C03 syllabus, from the Well-Architected Framework through networking, compute, storage, databases, security, and monitoring
- A consolidated topic review and a flashcard set
- Supporting reference material, including service maps and cheat sheets
- Obsidian templates used to maintain a consistent note structure

## Table of Contents

1. [Repository Structure](#repository-structure)
2. [Course Preparation and Resources](#1-course-preparation-and-resources)
3. [Note Taking with Obsidian](#2-note-taking-with-obsidian)
4. [What Helped Me Pass](#3-what-helped-me-pass)
5. [Exam Day](#4-exam-day)

## Repository Structure

```
0.study-notes/
  AWS-Training Notes/          Numbered topic notes (0 through 48)
  Attachements/                Diagrams and screenshots referenced by the notes
  Categories/                  Category index notes
  Daily Notes/                 Dated study logs
  Templates/                   Obsidian note templates
  files-tutorials-materials/   Cheat sheets and service reference maps
```

The notes are written in Markdown and are best viewed in [Obsidian](https://obsidian.md), which renders the internal links between topics. They remain readable in any Markdown viewer or directly on GitHub.

## 1. Course Preparation and Resources

### Background

My motivation for attempting this exam was to understand how AWS works and what cloud solutions it offers that could support my day to day work. I currently work as a Programmer Analyst and have built a range of solutions using Python, JavaScript, TypeScript, and Node. I also work with relational databases such as PostgreSQL and MySQL, so I brought a technical background and a working knowledge of software engineering to the exam preparation.

In terms of prior AWS experience, I was already familiar with several services, primarily through an experimental chatbot project I developed for my personal website. The services I had worked with beforehand included VPC, S3, KMS, Route 53, the AWS SDK, the AWS CLI, and Amazon Bedrock.

### Preparation Approach

My preparation began with video lectures provided by my organization. The lectures give a solid introduction to AWS services, but they do not cover each service's features, caveats, and appropriate use cases in depth. As an introduction, they are a reliable starting point.

I would recommend taking notes while watching the videos and reviewing those notes daily, or at least before starting a new lecture, so that each session builds on what has already been covered. In my assessment, video lectures give you a surface level understanding of how AWS works and contribute roughly 30 percent of your overall readiness.

A comparable share of your readiness comes from independent study and research. I would strongly recommend working through the [official AWS exam guide and study materials](https://docs.aws.amazon.com/aws-certification/latest/solutions-architect-associate-03/solutions-architect-associate-03.html) and conducting your own research into individual services. Independent study accounts for approximately another 30 percent of your readiness. This phase is oriented around your own study methodology and can be completed at your own pace. It is also the most dynamic phase, since you will be learning and researching continuously. This is where your written notes deliver the most value, allowing you to refresh your memory and encode new information efficiently. In my experience, regularly reviewing and revising the notes made a significant difference.

The remaining 40 percent comes from practice examinations and the structured reviews that follow them. Practice exams make a substantial difference, and I would **strongly recommend** beginning them as soon as you complete your video lectures.

Depending on the resources you use, your first few practice scores may fall below the threshold suggested by the practice platform's own scoring system. If you score below a passing grade, **do not be discouraged**. Continue studying. The reasons are as follows:

- **Practice exams are not scored the same way as the official AWS exam.** Practice platforms generally do not apply a weighted grading scheme and do not exclude unscored questions, whereas the official exam does.
- **The official exam contains 65 questions, of which 15 are unscored.** These 15 questions are used for evaluation purposes and are not identified as such. They appear exactly like any other question, so there is no way to distinguish them during the exam.
- **The passing score is 720 out of 1000,** and you are effectively graded on 50 questions.
- **The grading model can be confusing,** so I would recommend reviewing it yourself. The key takeaway is that a low first practice score is not a meaningful predictor of your final result.
- **Analyze every incorrect answer and understand why it was incorrect.** You need to know when and where each service is appropriate for a given scenario. Memorization alone will not carry you through scenario based questions. A strong conceptual understanding of each service is essential, and this is where independent research proves most valuable, since video lectures rarely cover the range of scenarios in sufficient depth.

Practice test reviews, topic based reviews, and flashcards all contribute considerably. They help you organize what you have learned and build your own ranking of which services are appropriate for each scenario. Taken together, video lectures, notes, independent research, practice tests, and reviews form a complete preparation path for someone approaching the exam without extensive prior AWS experience.

### Resources

There are many viable preparation paths and resources available. I would recommend consulting the community of fellow AWS candidates, who have already assembled an excellent collection of resources and guidance. The following community thread is a good starting point:

- [AWS Certified Solutions Architect Associate discussion, r/AWSCertifications](https://www.reddit.com/r/AWSCertifications/comments/1d5kkuw/aws_certified_solutions_architect_associate/)

The resources I used were:

| Resource                      | Type                | Provider                                |
| ----------------------------- | ------------------- | --------------------------------------- |
| Video lectures                | Instruction         | Storm Wind Studios, via my organization |
| Practice tests                | Assessment          | MeasureUp, via my organization          |
| Documentation and study guide | Reference           | AWS official documentation              |
| Generative AI assistants      | Review and quizzing | Claude, Gemini, ChatGPT                 |

Generative AI assistants proved **extremely** helpful for reviews and impromptu quizzing, subject to the caveats described in the next section.

## 2. Note Taking with Obsidian

I used Obsidian for note taking because it provides a flexible and versatile environment, supported by a strong community plugin ecosystem and robust linking between notes that makes relationships between topics explicit.

As reflected in this repository, the notes are extensively cross linked. This allows you to visualize how different services and their features relate to one another through the Obsidian graph view.

Obsidian also keeps notes well organized, and its community plugins support building and reviewing flashcards, connecting notes to AI assistants, and performing in depth search across the entire vault.

I revised my notes frequently, adding new information as I encountered it, since some services are deprecated or are not addressed in the video lectures. Details and supplementary features of each service need to be captured after the lectures, and Markdown notes offer the flexibility to do so efficiently.

One additional recommendation is to log the questions you answer incorrectly on practice tests and ask an AI assistant to help you understand the reasoning behind the correct answer and close any remaining knowledge gaps. AI assistants are genuinely useful, but they should not be relied on exclusively. Always verify their responses. I observed hallucinations when discussing several different services within a single chat session, so context window management matters. To manage AI context carefully, I connected my notes to Claude through Claude Code with read only access.

Below you can this repository's Obsidian knowledge graph. 

![Obsidian knowledge graph visualization](0.study-notes/Attachements/Pasted%20image%2020260908152638.png)

## 3. What Helped Me Pass

Taking practice tests and documenting the questions I answered incorrectly was the single most effective way to identify my weakest domains and remaining knowledge gaps.

One difficulty I encountered was that after analyzing my results, subsequent attempts at the same practice test triggered recall of the correct answers. This produces a false positive result, since remembering an answer does not indicate understanding of the underlying service. So I would recommend re-taking the practice exams at least a week later. 

Constant reviews and binge watching videos related to different AWS solutions helped me to recall my knowledge from my notes, and learn something new as well. Another great resource I leveraged was Generative AI. AI helps with analysis of your weak areas and provides easy to digest explanations and resources. 

## 4. Exam Day

On the day of the exam I reviewed my notes thoroughly and completed several rounds of flashcards, both the set I had built in Obsidian and open source Quizlet AWS flashcards. After completing those reviews, I sat the exam.

Time pressure during the actual exam is significant. Even at approximately two minutes per question, it feels as though you are running short on time. I would recommend managing your time deliberately and developing a strategy for how you approach each question before you sit down.

For final review, common exam traps, and guidance on identifying keywords within questions, I found the following repository useful:

- [aws-saa-c03-guides by RonitSachdev](https://github.com/RonitSachdev/aws-saa-c03-guides)

With a structured approach and consistent review, the exam is very achievable. I wish everyone taking it soon the best of luck.

## Use and Attribution

These notes are shared for the benefit of others preparing for the SAA-C03 examination. You are welcome to use, adapt, and extend them. They reflect the exam as I experienced it and the AWS service landscape at the time of writing, so please verify service details against the current [AWS documentation](https://docs.aws.amazon.com/).
