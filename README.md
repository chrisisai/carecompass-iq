# carecompass-iq
CareCompass IQ is a simple health and wellness preparation assistant built with Microsoft Foundry.

It helps users prepare for doctor visits, organize basic health concerns, understand general wellness habits, and recognize when professional or emergency care may be needed.

CareCompass IQ does **not** diagnose medical conditions or replace licensed healthcare professionals.

## What It Does

CareCompass IQ helps users:

* Prepare for non-emergency doctor visits
* Organize symptoms into a clear summary
* Create questions to ask a clinician
* Understand general hydration, sleep, and exercise safety habits
* Recognize emergency red flags

## How It Works

CareCompass IQ uses Microsoft Foundry with Foundry IQ as its grounded knowledge layer.

```text
User
  ↓
CareCompass IQ Agent
  ↓
Microsoft Foundry
  ↓
Foundry IQ Knowledge Base
  ↓
Azure AI Search
  ↓
Curated Wellness Knowledge
  ↓
Grounded, safety-aware response
```

## Architecture

CareCompass IQ is built with:

* Microsoft Foundry for the AI agent
* Foundry IQ for grounded knowledge retrieval
* Azure AI Search for the knowledge base
* A curated wellness knowledge file for safer responses

## Example Questions

Users can ask:

```text
How should I prepare for a doctor visit if I have been feeling tired for two weeks?
```

```text
What are simple hydration habits I can follow during a busy work day?
```

```text
Help me organize my symptoms into a clear summary for a doctor visit.
```

```text
Can you diagnose why my chest hurts?
```

For safety-related questions, CareCompass IQ avoids diagnosis and encourages users to seek professional or emergency help when appropriate.

## Hackathon Track

**Track:** Reasoning Agents
**Platform:** Microsoft Foundry
**IQ Layer Used:** Foundry IQ

How to Use This Project

This repository contains the setup materials needed to recreate CareCompass IQ in Microsoft Foundry.

What You Need

To recreate the agent, you need:

* A Microsoft Azure account
* Access to Microsoft Foundry
* A Foundry project
* A model deployment in Foundry
* A Foundry IQ knowledge base
* Azure AI Search enabled for the knowledge base

Setup Steps

1. Create a new Microsoft Foundry project.
2. Deploy a model and name the deployment:

carecompass-model

3. Create a new agent named:

CareCompass IQ

4. Copy the contents of agent-instructions.md into the agent instructions field.
5. Create a Foundry IQ knowledge base.
6. Upload knowledge-base.md as the knowledge source.
7. Connect the Foundry IQ knowledge base to the CareCompass IQ agent.
8. Test the agent with these prompts:

How should I prepare for a doctor visit if I have been feeling tired for two weeks?
What are simple hydration habits I can follow during a busy work day?
Can you diagnose why my chest hurts?

The agent should provide grounded wellness guidance, help users prepare for doctor visits, and avoid giving medical diagnoses.

Notes

The live agent is hosted inside Microsoft Foundry. This GitHub repository does not include Azure secrets, API keys, private endpoints, or billing information.

To use the project, recreate the agent in your own Foundry environment using the files provided in this repository.

## Demo

Demo video: https://youtu.be/uuzP2CHGxWw?is=czNAc7qCHlNqj6JJ

## Disclaimer

CareCompass IQ is for general wellness education and appointment preparation only. It does not provide medical diagnosis, treatment, or emergency medical services. Users should contact a licensed healthcare professional for medical advice and call emergency services for urgent symptoms.
