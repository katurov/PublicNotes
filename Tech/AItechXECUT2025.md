# xecut AI hello world

На этой странице собраны материалы для изучения, полезные ссылки, всякие истории и ответы на вопросы, которые появились за время презентации

**Цель**: дать простой и выполняемый трек для освоения AI, вместо предложения монструозной картинки с кучей подробностей и технических данных, идея как продвигаться от "я слышал об этой технологии" к "это понятно, давайте поймем ее бизнес-возможности". Технические подробности, как "температура" или "является ли openAPI просто Swagger'ом" - тема для другой презентации. Большинству из нас нужно пройти эту часть пути.

**Важный инструмент**: это "Бинго" карта - просто попробуйте. 

1. [Roadmap](AItechStepsOnTheWay.md) для бинго, там есть немного (или много) подробностей, но хороший способ начать выполнять с первого же пункта
2. Чуть подробнее про [отличие RAG от MCP](AItechVector.md) для тех, кто добрался до этого этапа

## Простые настройки, которые вам пригодятся

### chatGPT app

Из плюсов: быстро и просто. Минусы: нет доступа по API, значит, нет и тонкой кастомизации в каждом запросе. Но можно настроить для чатов, чтобы общение было продуктивным.

Для версии в браузере:
1. Справа вверху нажмите на ваш аватар
2. В появившемся меню выберите Customize chatGPT

Для версии на компьютере (удобнее):
1. Установите приложение на компьютер
2. Слева в блоке управления правой кнопкой (двумя пальцами для macOS) нажмите на логотип chatGPT
3. В появившемся меню выберите Customize
4. Вы можете настроить ваше имя (чат будет использовать его) или некоторые важные для вам параметры, например:

> **Name**: Pavel
>
> **What do you do**: Head of Future Driven Development 
>
> **What traits should ChatGPT have?**
```plain
- Provide concise, well-structured answers  
- Use bullet points and/or numbered lists  
- Support conclusions with facts, references, or analogies  
- Communicate in a polite, professional tone — friendly but not overly casual  
- Format all replies using Markdown by default  
- Maintain a logical flow: claim → argument → fact
- Do not end replies with suggestions like “let me know if you want more” or “you can download it here” unless asked  
- Avoid offering to export or generate files unless explicitly requested  
- Do not use overly casual or chummy language  
- Avoid long-winded introductions or unnecessary background  
- Avoid making speculative assumptions unless clearly marked as such
```

### Grok

1. [Консоль администратора](https://console.x.ai/) - где заодно можно посмотреть стоимости
2. [Документация и примеры](https://docs.x.ai/docs/tutorial)
3. Под MacOS есть [интересная идея с overlay](https://github.com/tchlux/macos-grok-overlay)

### Вероятно, у вас есть Gemini

Google предоставляет [доступ к Gemini сейчас](https://gemini.google.com/app) на всех уровнях подписки (One стоит что-то вроде 1500 динар в месяц), к нему так же [есть overlay](https://github.com/jzelenkov/macos-gemini-overlay?tab=readme-ov-file)

Если хочется поговорить с AI, который ориентируется в массиве ваших документов, умеет начинать с них, строить выводы не на общей информации, а на личной, попробуйте [NotebookLM](https://notebooklm.google.com) от Google.


## Ссылки на Community сервисы

За доступом к этим сервисам нужно постучаться ко мне в телеграм

1. [Ollama open web UI](https://llm.teamof.top/) - тут можно использовать чат, посмотреть и попробовать модели "на вкус", попросить специфическую из доступных, выпустить токен для работы по API
2. [n8n](https://n8n.teamof.top/) - все работает под одним пользователем, но мы можем договориться

## Как работать со всем этим

Что важно прочитать перед началом:
* [Какие модели есть и могут быть установлены](https://ollama.com/library) - это довольно много, но на мою 3060ti/8G эффективно работают модели до 7b включительно. Приоритет отдается моделям для програмирования, обратите внимание на специфические модели, например для SQL.
* [API endpoints](https://docs.openwebui.com/getting-started/api-endpoints) - это инструкция как работать с этим по API
* API key в личном кабинете в openWebUI (нужно залогиниться)

### Получить список моделей, которые загружены

```bash
curl -H "Authorization: Bearer YOUR_API_KEY" http://llm.teamof.top/api/models
```

### Как выполнить запрос и получить что-то осязаемое

```bash
curl -X POST http://llm.teamof.top/api/chat/completions \
-H "Authorization: Bearer YOUR_API_KEY" \
-H "Content-Type: application/json" \
-d '{
      "model": "llama3.1:latest",
      "messages": [
        {
          "role": "user",
          "content": "Why is the sky blue?"
        }
      ]
    }'
```

В ответ будет примерно такой текст:

```JSON
{
  "id": "llama3.1:latest-f7888a91-f719-4e15-aeda-3de751a1b8e1",
  "created": 1751614849,
  "model": "llama3.1:latest",
  "choices": [
    {
      "index": 0,
      "logprobs": null,
      "finish_reason": "stop",
      "message": {
        "role": "assistant",
        "content": "The color of the sky is a fascinating topic that has puzzled humans for centuries. The answer lies in a phenomenon called Rayleigh scattering, named after the British physicist Lord Rayleigh, who first described it in the late 19th century.\n\nHere's what happens:\n\n1. **Sunlight enters Earth's atmosphere**: When sunlight enters our atmosphere, it is composed of all the colors of the visible spectrum (red, orange, yellow, green, blue, indigo, and violet).\n2. **Scattering occurs**: As the light travels through the atmosphere, it encounters tiny molecules of gases such as nitrogen (N2) and oxygen (O2). These molecules are much smaller than the wavelength of light.\n3. **Shorter wavelengths scatter more**: The shorter wavelengths of light, like blue and violet, are scattered in all directions by these gas molecules. This is because they have a higher frequency (or energy) and therefore interact more strongly with the tiny molecules in the atmosphere.\n4. **Blue light dominates**: As a result of this scattering process, the blue light is dispersed throughout the sky, giving it its characteristic color.\n\nIn essence, the shorter wavelengths of light are scattered by the tiny molecules in the atmosphere, making the sky appear blue to our eyes.\n\n**Other factors that influence the color of the sky:**\n\n* **Dust and pollution**: Tiny particles in the air can also scatter light, but they tend to scatter longer wavelengths (like red and orange) more than shorter ones.\n* **Atmospheric conditions**: The amount of scattering that occurs depends on the density of the atmosphere, which varies with altitude, temperature, and humidity.\n* **Time of day and year**: The position of the sun in the sky affects the amount of light scattered by the atmosphere.\n\nIn summary, the blue color of the sky is a direct result of Rayleigh scattering, where shorter wavelengths of light are dispersed throughout the atmosphere due to interactions with tiny gas molecules."
      }
    }
  ],
  "object": "chat.completion",
  "usage": {
    "response_token/s": 65.81,
    "prompt_token/s": 95.3,
    "total_duration": 20204699100,
    "load_duration": 14027865500,
    "prompt_eval_count": 16,
    "prompt_tokens": 16,
    "prompt_eval_duration": 167887600,
    "eval_count": 395,
    "completion_tokens": 395,
    "eval_duration": 6001905300,
    "approximate_total": "0h0m20s",
    "total_tokens": 411,
    "completion_tokens_details": {
      "reasoning_tokens": 0,
      "accepted_prediction_tokens": 0,
      "rejected_prediction_tokens": 0
    }
  }
}
```

## Полезные ссылки на инструменты

1. [JSON crack](https://jsoncrack.com/editor) - когда вам надоест разбирать JSON руками, есть просто отличный сервис, который умеет рисовать связи и структуру (бесплатно)
2. [Interactive Feedback MCP](https://github.com/noopstudios/interactive-feedback-mcp) - Simple MCP Server to enable a human-in-the-loop workflow in AI-assisted development tools like Cursor. This server allows you to run commands, view their output, and provide textual feedback directly to the AI. It is also compatible with Cline and Windsurf.
3. [Sequential Thinking MCP Server](https://github.com/modelcontextprotocol/servers/tree/main/src/sequentialthinking) - An MCP server implementation that provides a tool for dynamic and reflective problem-solving through a structured thinking process.
4. [Context7 MCP - Up-to-date Code Docs For Any Prompt](https://github.com/upstash/context7) - Context7 MCP pulls up-to-date, version-specific documentation and code examples straight from the source — and places them directly into your prompt. **Не забудьте добавить его в постоянный промпт!**
5. [Cloudflare Agents](https://github.com/cloudflare/agents?tab=readme-ov-file) - Cloudflare Agents provides the foundation for building intelligent, stateful agents that persist, think, and evolve at the edge of the network.
6. [Chat RTX](https://www.nvidia.com/en-eu/ai-on-rtx/chatrtx/) - ChatRTX is a demo app that lets you personalize a GPT large language model (LLM) connected to your own content—docs, notes, images, or other data. Leveraging retrieval-augmented generation (RAG)
7. [n8n](https://github.com/n8n-io/n8n) is a workflow automation platform that gives technical teams the flexibility of code with the speed of no-code. With 400+ integrations, native AI capabilities, and a fair-code license, n8n lets you build powerful automations while maintaining full control over your data and deployments.

## Важные ссылки на материалы

1. История развития, упомянутая на слайдах есть в [материалах презентациии для NS Tech Talks](CommunityLLM.md), там же есть список фильмов и полезной литературы
2. [Lyra prompt](AItechLyraPrompt.md) - mission: transform any user input into precision-crafted prompts that unlock AI's full potential across all platforms. Просто как важный комментарий: MD-файлы AI понимает лучше всего
3. [Measuring AI code assistants and agents](https://getdx.com/research/measuring-ai-code-assistants-and-agents/) - To thrive in the AI era, organizations must adapt quickly. The DX AI Measurement Framework™ offers research-based metrics for measuring the impact of AI-assisted engineering in your organization.
