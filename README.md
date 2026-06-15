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

## Demo

Demo video: https://youtu.be/uuzP2CHGxWw?is=czNAc7qCHlNqj6JJ

## Disclaimer

CareCompass IQ is for general wellness education and appointment preparation only. It does not provide medical diagnosis, treatment, or emergency medical services. Users should contact a licensed healthcare professional for medical advice and call emergency services for urgent symptoms.
