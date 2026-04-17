# Interview Practice Roleplay

A Kilo-based roleplay simulation to help you practice for job interviews by simulating realistic interview scenarios.

## Overview

This project provides an interactive interview preparation tool using specialized AI agents. It includes:

- **Interview Master**: Orchestrates the interview session
- **Prep Specialist**: Analyzes job descriptions and resumes to generate tailored questions
- **Teaching Assistant**: Provides guidance and explanations when you struggle with answers

The system uses a collection of pre-defined interview questions and can generate custom plans based on your target role.

## Features

- Tailored interview questions based on job description and resume
- Real-time feedback and teaching during roleplay
- Support for technical and behavioral questions
- Difficulty levels: Easy, Medium, Hard
- Focus on Java/Spring ecosystem but extensible to other technologies

## Setup Requirements

- [Kilo CLI](https://kilo.ai/docs) installed
- Clone this repository
- Ensure the `.kilo/` directory is properly configured

## Usage

1. Provide your job description and resume to the Prep Specialist agent.
2. The system generates a personalized interview plan.
3. Start the roleplay with the Interview Master.
4. Answer questions; receive feedback and teaching as needed.

### Example Session

```
User: /agent interview-master
Kilo: Provide your job description and resume.
User: [uploads files]
Kilo: [Prep Specialist analyzes and generates plan]
Kilo: Let's begin. Question 1: [question]
```

## Project Structure

- `qb.instructions.md`: Contains sample interview questions
- `.github/agents/`: Agent definitions
  - `interview-master.agent.md`: Main orchestrator
  - `prep-me.agent.md`: Question generator
  - `teach-me.agent.md`: Teaching assistant
- `.github/prompts/qb.instructions.md`: Placeholder for generated questions

## Contributing

To add new questions:
1. Edit `qb.instructions.md` with new question blocks
2. Follow the format: Question Type, Technology/Skill, Question, Rationale, Difficulty, Expected Answer

To extend agents:
- Modify the agent `.md` files in `.github/agents/`
- Test changes with Kilo CLI

## License

See LICENSE file.
