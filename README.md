# Nextbit

**European AI inference for open-weight LLMs.**

Nextbit (NEXTBIT 256, S.L., Valencia, Spain) serves open-weight models such as Gemma, Qwen, DeepSeek and GLM through an OpenAI- and Anthropic-compatible API.

- **Serverless inference**: billed per token, no minimums
- **Dedicated endpoints**: single-tenant, fixed monthly fee
- **Fine-tuning** and **GPU cloud**
- **Private deployments** in your cloud or on-premise
- **EU-only endpoint** (`eu.api.nextbit256.com`): model inference runs exclusively on servers in the EU, with zero data retention of request content
- GDPR data processing agreement and EU AI Act model documentation

## Quickstart

Any OpenAI-compatible client works: change the base URL and the API key.

```python
from openai import OpenAI

client = OpenAI(
    base_url="https://eu.api.nextbit256.com/v1",
    api_key="YOUR_API_KEY",
)

response = client.chat.completions.create(
    model="gemma3:27b",
    messages=[{"role": "user", "content": "Hello!"}],
)
print(response.choices[0].message.content)
```

Models marked **EU** in the catalogue are available on the EU-only endpoint; models marked **Multi** run on the global endpoint (`api.nextbit256.com`).

## Links

- Website: https://www.nextbit256.com
- Models and pricing: https://www.nextbit256.com/en/models
- Documentation: https://www.nextbit256.com/en/docs/quickstart
- Terms of service: https://www.nextbit256.com/en/docs/terms-of-service
- X: https://x.com/Nextbit256
- LinkedIn: https://www.linkedin.com/company/nextbit256
