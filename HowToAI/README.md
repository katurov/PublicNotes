# Все то, что я знаю и читаю про ИИ (AI)

## Важная критика

3 April 2023 Rachel Metz ["AI Doesn’t Hallucinate. It Makes Things Up"](https://www.bloomberg.com/news/newsletters/2023-04-03/chatgpt-bing-and-bard-don-t-hallucinate-they-fabricate): 

> Humans have a tendency to anthropomorphize machines. (I have a robot vacuum named Randy.) But while ChatGPT and its ilk can produce convincing-sounding text, they don’t actually understand what they’re saying.
> 
> In this case, the term “hallucinate” obscures what’s really going on. It also serves to absolve the systems’ creators from taking responsibility for their products. (Oh, it’s not our fault, it’s just hallucinating!)
>
> Saying that a language model is hallucinating makes it sound as if it has a mind of its own that sometimes derails, said Giada Pistilli, principal ethicist at Hugging Face, which makes and hosts AI models.
> 
> “Language models do not dream, they do not hallucinate, they do not do psychedelics,” she wrote in an email. “It is also interesting to note that the word ‘hallucination’ hides something almost mystical, like mirages in the desert, and does not necessarily have a negative meaning as ‘mistake’ might.”

## Инструкции от первоисточников

* Original [Prompt engineering](https://platform.openai.com/docs/guides/prompt-engineering) ChatGPT (Dec. 2023): This guide shares strategies and tactics for getting better results from large language models (sometimes referred to as GPT models) like GPT-4. The methods described here can sometimes be deployed in combination for greater effect. We encourage experimentation to find the methods that work best for you.

* Отличный пост от Вастрики: [Кто побеждает в борьбе за технологии и что изменилось в AI с приходом опенсорса](https://vas3k.club/post/22008/). _Это история о дерзком гамбите Марка Цукерберга и мои размышления о том, как Бигтех компании будут делить рынок AI с Опенсорсом._

## Блоги

1. [Superhuman](https://superhuman.beehiiv.com) by Zain Kahn - Learn how to leverage AI to boost your productivity and accelerate your career. Join the world's biggest AI newsletter with 200,000+ readers from companies like Apple, Amazon, Google, Meta, Microsoft and more.
2. [The practical guide to using AI to do stuff](https://www.oneusefulthing.org/p/the-practical-guide-to-using-ai-to) by ETHAN MOLLICK - A resource for students in my classes (and other interested people). My classes now require AI (and if I didn’t require AI use, it wouldn’t matter, everyone is using AI anyway). But how can students use AI well? Here is a basic tutorial and guide I am providing my classes. It covers some of the many ways to use AI to be more productive, creative, and successful, using the technology available in early 2023, as well as some of the risks.
3. [AI Valley](https://www.theaivalley.com) - Join 50,000+ people discovering New AI Tools, Useful Prompts, and Latest AI Developments | Read by professionals from Google, OpenAI, Notion, Apple. 
4. [Китайская комната](https://ru.wikipedia.org/wiki/Китайская_комната) - важное объяснение, как это работает. 
5. [Ложная слепота](https://fantlab.ru/work134421) by Питер Уоттс - научная фантастика о том, как люди сталкиваются с ИИ
6. [The Ultimate GPT-4 Guide](https://hasantoxr.gumroad.com/l/gpt4) by [Hasan Toor](https://bio.link/hasantoxr) - Learn and Master everything about GPT-4 to enhance and level up your life. 
7. [Benchmarking](https://www.youtube.com/watch?v=ZnhFA-r_YvA) of GPU, а так же в практическом применении [RTX 2060 Vs GTX 1080Ti Deep Learning Benchmarks: Cheapest RTX card Vs Most Expensive GTX card](https://towardsdatascience.com/rtx-2060-vs-gtx-1080ti-in-deep-learning-gpu-benchmarks-cheapest-rtx-vs-most-expensive-gtx-card-cd47cd9931d2).
8. Техническая спецификация от [rtx-3070-3070ti](https://www.nvidia.com/en-eu/geforce/graphics-cards/30-series/rtx-3070-3070ti/), которая стоит примерно 94 000 динар
9. [A collection of AWESOME things about Graph-Related Large Language Models (LLMs)](https://github.com/XiaoxinHe/Awesome-Graph-LLM)

## Инструменты и программы

1. [chatGPT](https://chat.openai.com)
2. [DiffusionBee](https://diffusionbee.com) - DiffusionBee is the easiest way to generate AI art on your computer with Stable Diffusion. Completely free of charge. Runs offline. No limits. [Он на Гит](https://github.com/divamgupta/diffusionbee-stable-diffusion-ui). В него можно загружать разные модели [по инструкции](https://github.com/divamgupta/diffusionbee-stable-diffusion-ui/blob/master/DOCUMENTATION.md) из [huggingface](https://huggingface.co/models?other=stable-diffusion), в том числе и [midjourney-v4-diffusion](https://huggingface.co/flax/midjourney-v4-diffusion).
3. [How to Run Stable Diffusion Locally With a GUI on Windows](https://www.howtogeek.com/832491/how-to-run-stable-diffusion-locally-with-a-gui-on-windows/) - This fork also contains various optimizations that should allow it to run on PCs with less RAM, built-in upscaling and facial capabilities using GFPGAN, ESRGAN, RealESRGAN, and CodeFormer, and masking. Masking is a huge deal — it allows you to selectively apply the AI image generation to certain parts of the image without distorting other parts, a process typically called inpainting. Но стоит внимательно смотреть на системные требования.
4. [Easy Diffusion](https://stable-diffusion-ui.github.io) - можно установить на сервер и использовать вместе с друзьями и коллегами. Можно загрузить модели [по инструкции](https://github.com/divamgupta/diffusionbee-stable-diffusion-ui/blob/master/DOCUMENTATION.md) из [huggingface](https://huggingface.co/models?other=stable-diffusion), в том числе и [midjourney-v4-diffusion](https://huggingface.co/flax/midjourney-v4-diffusion).
5. [photofeeler](https://www.photofeeler.com) - программа, которая описывает фото параметрически, какое подойдет для резюме, а что - для службы знакомств
6. [whisper.cpp](https://github.com/ggerganov/whisper.cpp) - M1 версия [Whisper](https://github.com/openai/whisper/tree/main), программы по распознанию текста из речи
7. [llama.cpp](https://github.com/ggerganov/llama.cpp) - M1 версия [LLaMA](https://arxiv.org/abs/2302.13971): Open and Efficient Foundation Language Models. We introduce LLaMA, a collection of foundation language models ranging from 7B to 65B parameters. We train our models on trillions of tokens, and show that it is possible to train state-of-the-art models using publicly available datasets exclusively, without resorting to proprietary and inaccessible datasets. In particular, LLaMA-13B outperforms GPT-3 (175B) on most benchmarks, and LLaMA-65B is competitive with the best models, Chinchilla-70B and PaLM-540B. We release all our models to the research community. Очень важно внутрь положить оригинальные файлы (magnet:?xt=urn:btih:b8287ebfa04f879b048d4d4404108cf3e8014352&dn=LLaMA) LLaMA [по инструкции](https://github.com/facebookresearch/llama/issues/149)
8. [krisp](https://krisp.ai) - improves the productivity of online meetings with it’s AI-powered Voice Clarity and Meeting Assistant. Есть бесплатный тариф, но вообще [за деньги](https://krisp.ai/pricing/). Главный промо из двух частей: чистит звук, выступая виртуальным девайсом; умеет расшифровать текст, но только английский (вот и чего не wisper, который умеет и русский?). Интересно, что этот стартап [из Армении](https://www.forbes.ru/rubriki-kanaly/video/490322-kak-relokanty-iz-rossii-vliaut-na-ekonomiku-armenii)
9. [uizard](https://uizard.io) - помогает нарисовать интерфейс для программы. Киллер-фича - возможность загрузить скриншот, который будет распознан в элементы и после этого доступен для редактирования, словно его перерисовали. Так же обладает возможностью интерактива: можно связывать элементы для перехода, что отлично работает во время демонатрации будущих возможностей. Идеально для обсуждения изменений в программы
10. [tl;dv](https://tldv.io) - облако, программа и модули для популярных клиентов видеоконференций (например, zoom), помогает получить запись и расшифровку встречи. Плюсы: понимает по русски. Минусы: облако, хочет денег. **Важно**: во время встречи позволяет сделать короткие заметки, как таймкоды, которые после умеет использовать для навигации по видео и тексту. Это интересное приложение, точно стоит его пробовать.
11. [Remove even the most annoying watermarks from images for free](https://dewatermark.ai) - делает ровно то, что заявлено (удаляет ватермарки). Обещают сервис бесплатным на протяжении всего времени. В комплекте еще три тулзы: [Remove-BG.ai](https://remove-bg.ai) убирает фон на фото, [UP-scales.ai](https://upscales.ai) ап-скейлит изображения, [passportmaker.ai](https://passportmaker.ai) из просто фото делает "паспортное" (внезапный сервис, конечно).
12. [What Is Chat with RTX?](https://www.nvidia.com/en-us/ai-on-rtx/chat-with-rtx-generative-ai/) Chat With RTX is a demo app that lets you personalize a GPT large language model (LLM) connected to your own content—docs, notes, videos, or other data. Leveraging retrieval-augmented generation (RAG), TensorRT-LLM, and RTX acceleration, you can query a custom chatbot to quickly get contextually relevant answers. And because it all runs locally on your Windows RTX PC or workstation, you’ll get fast and secure results.
13. [Make the most of your new mind](https://mymind.com/videos) - система для сохранения информации из разных источников (совсем разных, от текста до видео и картинок), с последующей автоматической кластеризацией (по неизвестному алгоритму). Пока неясно, как работает с русским языком. Строго платно.

## Важная ремарка про GPU

[Mou](https://github.com/mou) правильно подсказал, что benchmark от геймеров не вполне отражает производительность в задачах ИИ, так что важнее смотреть на количество CUDA ядер, скорость памяти и т.п. При этом нужно оценить минимум памяти карты, судя по всему, это от 6G (меньше моделей просто нет).

[Сами nVidea](https://www.youtube.com/watch?v=L6rJA0z2Kag) про себя и смысл всего этого в интересном ролике

В требованиях к "Chat with RTX" NVIDIA описывает требования к карте, как
> NVIDIA GeForce™ RTX 30 or 40 Series GPU or NVIDIA RTX™ Ampere or Ada Generation GPU with at least 8GB of VRAM
на что и следует ориентироваться сегодня

## Про программирование

1. [Деревья решений](https://scikit-learn.ru/1-10-decision-trees/) - это непараметрический контролируемый метод обучения, используемый для классификации и регрессии . Цель состоит в том, чтобы создать модель, которая предсказывает значение целевой переменной, изучая простые правила принятия решений, выведенные из характеристик данных. Дерево можно рассматривать как кусочно-постоянное приближение.
2. [How To Use GPU with PyTorch](https://wandb.ai/wandb/common-ml-errors/reports/How-To-Use-GPU-with-PyTorch---VmlldzozMzAxMDk) by Ayush Thakur - A short tutorial on using GPUs for your deep learning models with PyTorch, from checking availability to visualizing usable. 
```
>>> import torch
>>> torch.cuda.is_available()
```
3. [pyllama](https://github.com/juncongmoo/pyllama) - 📢 pyllama is a hacked version of LLaMA based on original Facebook's implementation but more convenient to run in a Single consumer grade GPU.
```
pip install pyllama -U
```
## For Apple

1. Apple machine learning research [released](https://twitter.com/awnihannun/status/1732184443451019431) Apple' silicon [native MLX](https://github.com/ml-explore/mlx) and [the documentation](https://ml-explore.github.io/mlx/build/html/quick_start.html) for lots of things like:
  * Transformer language model training.
  * Large-scale text generation with LLaMA and finetuning with LoRA.
  * Generating images with Stable Diffusion.
  * Speech recognition with OpenAI's Whisper.
