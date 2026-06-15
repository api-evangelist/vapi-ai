# Vapi (vapi-ai)

Vapi is a San Francisco-based voice AI platform that lets developers build real-time, low-latency voice agents over phone, web, and SIP. It orchestrates three modular components — a transcriber (STT), an LLM, and a voice (TTS) — into a sub-700ms voice-to-voice pipeline, with first-class support for tools/function calling, multi-agent squads, outbound campaigns, persistent sessions, structured outputs, recording artifacts, evaluation scorecards, and a full REST API plus official SDKs in TypeScript, Python, C#, Ruby, PHP, and client SDKs for Web, React Native, iOS, and Python. Vapi is a Y Combinator company.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/apis.yml)

## Scope

- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

- AI
- Voice AI
- Voice Agents
- Conversational AI
- Telephony
- Real-Time
- Transcription
- Text-to-Speech
- LLM
- Agents
- MCP

## Timestamps

- **Created:** 2026-05-24T00:00:00.000Z
- **Modified:** 2026-05-29

## APIs

### Vapi Assistants API

Create and manage Vapi voice assistants. An assistant bundles a transcriber, LLM, voice (TTS), server URL, tools, first message, system prompt, voicemail handling, and call analysis plan into a reusable voice agent configuration that can be attached to inbound or outbound phone numbers, web calls, or squads.

- **Human URL:** [https://docs.vapi.ai/api-reference/assistants/list](https://docs.vapi.ai/api-reference/assistants/list)

#### Tags

- Assistants
- Voice AI
- Agents

#### Properties

- [Documentation](https://docs.vapi.ai/api-reference/assistants/list)
- [OpenAPI](openapi/vapi-assistants-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/vapi-assistants-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vapi-assistants-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/vapi-assistant-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/vapi-assistant-structure.json)
- [Example](examples/vapi-assistant-example.json)

### Vapi Calls API

Create outbound calls, accept inbound calls, list and filter calls, fetch call status and analysis, delete call data, and download per-call artifacts including mono and stereo recordings, customer/assistant isolated recordings, video recordings, PCAP packet captures, and structured call logs.

- **Human URL:** [https://docs.vapi.ai/api-reference/calls/list](https://docs.vapi.ai/api-reference/calls/list)

#### Tags

- Calls
- Voice AI
- Telephony

#### Properties

- [Documentation](https://docs.vapi.ai/api-reference/calls/list)
- [OpenAPI](openapi/vapi-calls-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/vapi-calls-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vapi-calls-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/vapi-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [JSON Schema](json-schema/vapi-call-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/vapi-call-structure.json)
- [Example](examples/vapi-call-example.json)

### Vapi Phone Numbers API

Buy, BYO-import, and manage phone numbers from Vapi (vapi.phoneNumber), Twilio, Telnyx, Vonage, and SIP trunks. Attach an assistant or squad to a number for inbound routing and configure outbound caller-id behavior.

- **Human URL:** [https://docs.vapi.ai/api-reference/phone-numbers/list](https://docs.vapi.ai/api-reference/phone-numbers/list)

#### Tags

- Phone Numbers
- Telephony
- Voice AI

#### Properties

- [Documentation](https://docs.vapi.ai/api-reference/phone-numbers/list)
- [OpenAPI](openapi/vapi-phone-numbers-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/vapi-phone-numbers-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vapi-phone-numbers-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/vapi-phone-number-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/vapi-phone-number-structure.json)
- [Example](examples/vapi-phone-number-example.json)

### Vapi Squads API

Compose multiple assistants into a Squad — a multi-agent workflow where the active assistant can hand off a live call to another assistant in the squad based on tools, intents, or transfer destinations.

- **Human URL:** [https://docs.vapi.ai/api-reference/squads/list](https://docs.vapi.ai/api-reference/squads/list)

#### Tags

- Squads
- Voice AI
- Agents

#### Properties

- [Documentation](https://docs.vapi.ai/api-reference/squads/list)
- [OpenAPI](openapi/vapi-squads-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/vapi-squads-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vapi-squads-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Vapi Tools API

Define and manage Tools (function tools, transfer-call tools, end-call tools, DTMF tools, hangup tools, voicemail tools, MCP tools, query tools, Make/Zapier tools, knowledge-base tools, and Google/Slack/ GoHighLevel integrations) that the assistant LLM can invoke during a call.

- **Human URL:** [https://docs.vapi.ai/api-reference/tools/list](https://docs.vapi.ai/api-reference/tools/list)

#### Tags

- Tools
- Voice AI
- Function Calling

#### Properties

- [Documentation](https://docs.vapi.ai/api-reference/tools/list)
- [OpenAPI](openapi/vapi-tools-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/vapi-tools-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vapi-tools-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Vapi Files API

Upload, list, retrieve, update, and delete files used as inputs to knowledge bases and other assistant-side artifacts.

- **Human URL:** [https://docs.vapi.ai/api-reference/files/list](https://docs.vapi.ai/api-reference/files/list)

#### Tags

- Files
- Voice AI
- Knowledge Base

#### Properties

- [Documentation](https://docs.vapi.ai/api-reference/files/list)
- [OpenAPI](openapi/vapi-files-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/vapi-files-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vapi-files-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Vapi Chats API

Text-based conversation surface that reuses the same assistant configuration as voice calls, including an OpenAI-compatible /chat/responses endpoint for drop-in replacement of OpenAI chat completions.

- **Human URL:** [https://docs.vapi.ai/api-reference/chats/list](https://docs.vapi.ai/api-reference/chats/list)

#### Tags

- Chats
- Voice AI
- Text

#### Properties

- [Documentation](https://docs.vapi.ai/api-reference/chats/list)
- [OpenAPI](openapi/vapi-chats-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/vapi-chats-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vapi-chats-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Vapi Sessions API

Stateful sessions that persist conversation history across calls and chats so an assistant can pick up where the customer left off.

- **Human URL:** [https://docs.vapi.ai/api-reference/sessions/list](https://docs.vapi.ai/api-reference/sessions/list)

#### Tags

- Sessions
- Voice AI
- State

#### Properties

- [Documentation](https://docs.vapi.ai/api-reference/sessions/list)
- [OpenAPI](openapi/vapi-sessions-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/vapi-sessions-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vapi-sessions-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Vapi Campaigns API

Outbound calling campaigns — upload a customer list and schedule batched outbound calls against one or more assistants and phone numbers with concurrency and retry policies.

- **Human URL:** [https://docs.vapi.ai/api-reference/campaigns/list](https://docs.vapi.ai/api-reference/campaigns/list)

#### Tags

- Campaigns
- Voice AI
- Outbound

#### Properties

- [Documentation](https://docs.vapi.ai/api-reference/campaigns/list)
- [OpenAPI](openapi/vapi-campaigns-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/vapi-campaigns-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vapi-campaigns-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Vapi Analytics API

Run aggregate analytics queries across calls — group by assistant, time bucket, status, end-reason, success evaluation, cost, and duration — for dashboards and chargeback reporting.

- **Human URL:** [https://docs.vapi.ai/api-reference/analytics/create](https://docs.vapi.ai/api-reference/analytics/create)

#### Tags

- Analytics
- Voice AI
- Reporting

#### Properties

- [Documentation](https://docs.vapi.ai/api-reference/analytics/create)
- [OpenAPI](openapi/vapi-analytics-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/vapi-analytics-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vapi-analytics-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Vapi Insight API

Define and run Insight queries across call data, including preview-before-save and on-demand runs, to extract structured signals from conversation transcripts.

- **Human URL:** [https://docs.vapi.ai/api-reference/insights/list](https://docs.vapi.ai/api-reference/insights/list)

#### Tags

- Insight
- Voice AI
- Observability

#### Properties

- [Documentation](https://docs.vapi.ai/api-reference/insights/list)
- [OpenAPI](openapi/vapi-insight-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/vapi-insight-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vapi-insight-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Vapi Observability Scorecard API

Define LLM-graded scorecards that automatically evaluate every call against your defined success criteria and produce structured scores for trend analysis and regression detection.

- **Human URL:** [https://docs.vapi.ai/api-reference/scorecards/list](https://docs.vapi.ai/api-reference/scorecards/list)

#### Tags

- Observability
- Scorecard
- Voice AI
- Evaluation

#### Properties

- [Documentation](https://docs.vapi.ai/api-reference/scorecards/list)
- [OpenAPI](openapi/vapi-observability-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/vapi-observability-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vapi-observability-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Vapi Eval API

Create test suites that simulate end-user behavior against an assistant, run them on demand, and inspect per-run pass/fail and judge output for regression testing of voice agents.

- **Human URL:** [https://docs.vapi.ai/api-reference/evals/list](https://docs.vapi.ai/api-reference/evals/list)

#### Tags

- Eval
- Voice AI
- Testing

#### Properties

- [Documentation](https://docs.vapi.ai/api-reference/evals/list)
- [OpenAPI](openapi/vapi-eval-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/vapi-eval-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vapi-eval-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Vapi Structured Outputs API

Define JSON-Schema-driven structured outputs that the assistant must populate from a call, plus an on-demand /structured-output/run endpoint to backfill outputs against an existing transcript.

- **Human URL:** [https://docs.vapi.ai/api-reference/structured-outputs/list](https://docs.vapi.ai/api-reference/structured-outputs/list)

#### Tags

- Structured Outputs
- Voice AI

#### Properties

- [Documentation](https://docs.vapi.ai/api-reference/structured-outputs/list)
- [OpenAPI](openapi/vapi-structured-outputs-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/vapi-structured-outputs-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vapi-structured-outputs-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Vapi Provider Resources API

Generic CRUD over provider-side resources (e.g. ElevenLabs voices, Cartesia voices, Deepgram custom models) so they can be created and managed through Vapi without leaving the platform.

- **Human URL:** [https://docs.vapi.ai/api-reference/provider-resources/list](https://docs.vapi.ai/api-reference/provider-resources/list)

#### Tags

- Provider Resources
- Voice AI
- Integrations

#### Properties

- [Documentation](https://docs.vapi.ai/api-reference/provider-resources/list)
- [OpenAPI](openapi/vapi-provider-resources-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/vapi-provider-resources-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vapi-provider-resources-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Arazzo Workflows](arazzo/) — [Arazzo Specification](https://spec.openapis.org/arazzo/latest.html)
- [Portal](https://vapi.ai)
- [Documentation](https://docs.vapi.ai)
- [Documentation](https://api.vapi.ai/api)
- [OpenAPI](https://api.vapi.ai/api-json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Getting Started](https://docs.vapi.ai/quickstart)
- [Sign Up](https://dashboard.vapi.ai)
- [Status Page](https://status.vapi.ai)
- [Pricing](https://vapi.ai/pricing)
- [Forum](https://discord.gg/pUFNcf2WmH)
- [Blog](https://vapi.ai/blog)
- [Changelog](https://vapi.ai/changelog)
- [GitHub Organization](https://github.com/VapiAI)
- [SDK](https://github.com/VapiAI/server-sdk-typescript)
- [SDK](https://github.com/VapiAI/server-sdk-python)
- [SDK](https://github.com/VapiAI/server-sdk-csharp)
- [SDK](https://github.com/VapiAI/server-sdk-ruby)
- [SDK](https://github.com/VapiAI/server-sdk-php)
- [SDK](https://github.com/VapiAI/client-sdk-web)
- [SDK](https://github.com/VapiAI/client-sdk-python)
- [SDK](https://github.com/VapiAI/client-sdk-react-native)
- [SDK](https://github.com/VapiAI/client-sdk-ios)
- [SDK](https://github.com/VapiAI/client-sdk-html-script-tag)
- [Tool](https://github.com/VapiAI/mcp-server)
- [Tool](https://github.com/VapiAI/skills)
- [Tool](https://github.com/VapiAI/gitops)
- [Code Examples](https://github.com/VapiAI/docs)
- [Webhooks](https://docs.vapi.ai/server-url)
- [Webhooks](https://docs.vapi.ai/server-url/events)
- [AsyncAPI](asyncapi/vapi-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [Trust Center](https://trust.vapi.ai)
- [Privacy Policy](https://vapi.ai/privacy)
- [Terms of Service](https://vapi.ai/terms-of-service)
- [Terms of Service](https://vapi.ai/aup)
- [Twitter](https://x.com/Vapi_AI)
- [LinkedIn](https://www.linkedin.com/company/vapi-ai)
- [Documentation](https://www.ycombinator.com/companies/vapi)
- [Plans](plans/vapi-ai-plans-pricing.yml)
- [Rate Limits](rate-limits/vapi-ai-rate-limits.yml)
- [Fin Ops](finops/vapi-ai-finops.yml)
- [Features](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
