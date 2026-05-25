# Vapi (vapi-ai)
Vapi is a San Francisco-based voice AI platform that lets developers build real-time, low-latency voice agents over phone, web, and SIP. It orchestrates three modular components — a transcriber (STT), an LLM, and a voice (TTS) — into a sub-700ms voice-to-voice pipeline, with first-class support for tools/function calling, multi-agent squads, outbound campaigns, persistent sessions, structured outputs, recording artifacts, evaluation scorecards, and a full REST API plus official SDKs.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

 - AI, Voice AI, Voice Agents, Conversational AI, Telephony, Real-Time, Transcription, Text-to-Speech, LLM, Agents, MCP

## Timestamps

- **Created:** 2026-05-24
- **Modified:** 2026-05-24

## Architecture

Vapi is an orchestration layer over three modules: the **transcriber**, the **model**, and the **voice**. Multiple providers are supported for each module (Deepgram, AssemblyAI, Cartesia, Gladia, Soniox, Speechmatics, Azure, Google, OpenAI for STT; OpenAI, Anthropic, Google, xAI, Groq, DeepSeek and more for LLM; ElevenLabs, Cartesia, PlayHT, OpenAI, Azure, Deepgram, Rime and more for TTS). Pricing is $0.05/min for Vapi's orchestration plus pass-through provider cost (or $0 if you BYO keys).

## APIs

### Vapi Assistants API
Create and manage Vapi voice assistants — reusable bundles of transcriber, LLM, voice, tools, prompts, and analysis configuration.

**Human URL:** [https://docs.vapi.ai/api-reference/assistants/list](https://docs.vapi.ai/api-reference/assistants/list)

- [OpenAPI](openapi/vapi-assistants-api-openapi.yml)
- [JSON Schema](json-schema/vapi-assistant-schema.json)
- [JSON Structure](json-structure/vapi-assistant-structure.json)
- [Example](examples/vapi-assistant-example.json)
- [Naftiko Capability](capabilities/assistants-assistants.yaml)

### Vapi Calls API
Create outbound calls, accept inbound calls, list calls, fetch status, delete call data, and download per-call recordings, PCAP packet captures, and call logs.

**Human URL:** [https://docs.vapi.ai/api-reference/calls/list](https://docs.vapi.ai/api-reference/calls/list)

- [OpenAPI](openapi/vapi-calls-api-openapi.yml)
- [JSON Schema](json-schema/vapi-call-schema.json)
- [JSON Structure](json-structure/vapi-call-structure.json)
- [Example](examples/vapi-call-example.json)
- [Naftiko Capability](capabilities/calls-calls.yaml)

### Vapi Phone Numbers API
Buy, BYO-import, and manage phone numbers from Vapi, Twilio, Telnyx, Vonage, and SIP trunks. Attach an assistant or squad to a number for inbound routing.

**Human URL:** [https://docs.vapi.ai/api-reference/phone-numbers/list](https://docs.vapi.ai/api-reference/phone-numbers/list)

- [OpenAPI](openapi/vapi-phone-numbers-api-openapi.yml)
- [JSON Schema](json-schema/vapi-phone-number-schema.json)
- [Naftiko Capability](capabilities/phone-numbers-phone-numbers.yaml)

### Vapi Squads API
Compose multiple assistants into a Squad — a multi-agent workflow with mid-call handoff between specialized assistants.

**Human URL:** [https://docs.vapi.ai/api-reference/squads/list](https://docs.vapi.ai/api-reference/squads/list)

- [OpenAPI](openapi/vapi-squads-api-openapi.yml)
- [Naftiko Capability](capabilities/squads-squads.yaml)

### Vapi Tools API
Function tools, transfer-call, end-call, DTMF, hangup, voicemail, MCP, query, Make/Zapier, Slack/GHL, knowledge-base, and more.

**Human URL:** [https://docs.vapi.ai/api-reference/tools/list](https://docs.vapi.ai/api-reference/tools/list)

- [OpenAPI](openapi/vapi-tools-api-openapi.yml)
- [JSON Schema](json-schema/vapi-tool-schema.json)
- [Naftiko Capability](capabilities/tools-tools.yaml)

### Vapi Files API
Upload, list, retrieve, update, and delete files used as inputs to knowledge bases and other assistant-side artifacts.

**Human URL:** [https://docs.vapi.ai/api-reference/files/list](https://docs.vapi.ai/api-reference/files/list)

- [OpenAPI](openapi/vapi-files-api-openapi.yml)
- [Naftiko Capability](capabilities/files-files.yaml)

### Vapi Chats API
Text-based conversation surface that reuses the assistant configuration as voice calls, including an OpenAI-compatible `/chat/responses` endpoint.

**Human URL:** [https://docs.vapi.ai/api-reference/chats/list](https://docs.vapi.ai/api-reference/chats/list)

- [OpenAPI](openapi/vapi-chats-api-openapi.yml)
- [Naftiko Capability](capabilities/chats-chats.yaml)

### Vapi Sessions API
Stateful sessions that persist conversation history across calls and chats.

**Human URL:** [https://docs.vapi.ai/api-reference/sessions/list](https://docs.vapi.ai/api-reference/sessions/list)

- [OpenAPI](openapi/vapi-sessions-api-openapi.yml)
- [Naftiko Capability](capabilities/sessions-sessions.yaml)

### Vapi Campaigns API
Outbound calling campaigns with concurrency and retry policies.

**Human URL:** [https://docs.vapi.ai/api-reference/campaigns/list](https://docs.vapi.ai/api-reference/campaigns/list)

- [OpenAPI](openapi/vapi-campaigns-api-openapi.yml)
- [Naftiko Capability](capabilities/campaigns-campaigns.yaml)

### Vapi Analytics API
Aggregate analytics queries across calls.

**Human URL:** [https://docs.vapi.ai/api-reference/analytics/create](https://docs.vapi.ai/api-reference/analytics/create)

- [OpenAPI](openapi/vapi-analytics-api-openapi.yml)
- [Naftiko Capability](capabilities/analytics-analytics.yaml)

### Vapi Insight API
Define and run Insight queries to extract structured signals from call transcripts.

**Human URL:** [https://docs.vapi.ai/api-reference/insights/list](https://docs.vapi.ai/api-reference/insights/list)

- [OpenAPI](openapi/vapi-insight-api-openapi.yml)
- [Naftiko Capability](capabilities/insight-insight.yaml)

### Vapi Observability Scorecard API
LLM-graded scorecards that automatically evaluate every call against your success criteria.

**Human URL:** [https://docs.vapi.ai/api-reference/scorecards/list](https://docs.vapi.ai/api-reference/scorecards/list)

- [OpenAPI](openapi/vapi-observability-api-openapi.yml)
- [Naftiko Capability](capabilities/observability-observability.yaml)

### Vapi Eval API
Test suites that simulate end-user behavior against an assistant for regression testing.

**Human URL:** [https://docs.vapi.ai/api-reference/evals/list](https://docs.vapi.ai/api-reference/evals/list)

- [OpenAPI](openapi/vapi-eval-api-openapi.yml)
- [Naftiko Capability](capabilities/eval-eval.yaml)

### Vapi Structured Outputs API
JSON-Schema-driven structured outputs from a call, plus on-demand backfill.

**Human URL:** [https://docs.vapi.ai/api-reference/structured-outputs/list](https://docs.vapi.ai/api-reference/structured-outputs/list)

- [OpenAPI](openapi/vapi-structured-outputs-api-openapi.yml)
- [Naftiko Capability](capabilities/structured-outputs-structured-outputs.yaml)

### Vapi Provider Resources API
Generic CRUD over upstream provider resources (e.g. ElevenLabs voices, Cartesia voices, Deepgram custom models).

**Human URL:** [https://docs.vapi.ai/api-reference/provider-resources/list](https://docs.vapi.ai/api-reference/provider-resources/list)

- [OpenAPI](openapi/vapi-provider-resources-api-openapi.yml)
- [Naftiko Capability](capabilities/provider-resources-provider-resources.yaml)

## Authentication

Bearer token in the `Authorization` header. Get your API key from the [Vapi Dashboard](https://dashboard.vapi.ai).

```
Authorization: Bearer <VAPI_API_KEY>
```

## Pricing

- **Build** — usage-based: $0.05/min Vapi orchestration, $10/line/month above 10 included concurrent lines, $0.005/SMS, provider costs pass-through (or $0 with BYOK)
- **Scale** — annual contract with custom volume pricing, SOC 2, PCI, SSO, RBAC, SLA
- **HIPAA Add-on** — $2,000/month
- **Zero Data Retention Add-on** — $1,000/month

See [plans/vapi-ai-plans-pricing.yml](plans/vapi-ai-plans-pricing.yml), [rate-limits/vapi-ai-rate-limits.yml](rate-limits/vapi-ai-rate-limits.yml), and [finops/vapi-ai-finops.yml](finops/vapi-ai-finops.yml).

## SDKs and Tools

**Server SDKs:** [TypeScript](https://github.com/VapiAI/server-sdk-typescript) · [Python](https://github.com/VapiAI/server-sdk-python) · [C#](https://github.com/VapiAI/server-sdk-csharp) · [Ruby](https://github.com/VapiAI/server-sdk-ruby) · [PHP](https://github.com/VapiAI/server-sdk-php)

**Client SDKs:** [Web](https://github.com/VapiAI/client-sdk-web) · [Python](https://github.com/VapiAI/client-sdk-python) · [React Native](https://github.com/VapiAI/client-sdk-react-native) · [iOS](https://github.com/VapiAI/client-sdk-ios) · [HTML Script Tag](https://github.com/VapiAI/client-sdk-html-script-tag)

**Tools:** [Vapi MCP Server](https://github.com/VapiAI/mcp-server) · [Vapi Skills](https://github.com/VapiAI/skills) · [Vapi GitOps](https://github.com/VapiAI/gitops)

## Links

- [Portal](https://vapi.ai)
- [Docs](https://docs.vapi.ai)
- [Swagger UI](https://api.vapi.ai/api)
- [Raw OpenAPI JSON](https://api.vapi.ai/api-json)
- [Status](https://status.vapi.ai)
- [Dashboard](https://dashboard.vapi.ai)
- [Trust Center](https://trust.vapi.ai)
- [GitHub](https://github.com/VapiAI)
- [Discord](https://discord.gg/pUFNcf2WmH)
