# Все то, что я знаю и читаю про ИИ (AI)

## Блоги

1. [Superhuman](https://superhuman.beehiiv.com) by Zain Kahn - Learn how to leverage AI to boost your productivity and accelerate your career. Join the world's biggest AI newsletter with 200,000+ readers from companies like Apple, Amazon, Google, Meta, Microsoft and more.
2. [The practical guide to using AI to do stuff](https://www.oneusefulthing.org/p/the-practical-guide-to-using-ai-to) by ETHAN MOLLICK - A resource for students in my classes (and other interested people). My classes now require AI (and if I didn’t require AI use, it wouldn’t matter, everyone is using AI anyway). But how can students use AI well? Here is a basic tutorial and guide I am providing my classes. It covers some of the many ways to use AI to be more productive, creative, and successful, using the technology available in early 2023, as well as some of the risks.
3. [AI Valley](https://www.theaivalley.com) - Join 50,000+ people discovering New AI Tools, Useful Prompts, and Latest AI Developments | Read by professionals from Google, OpenAI, Notion, Apple. 
4. [Китайская комната](https://ru.wikipedia.org/wiki/Китайская_комната) - важное объяснение, как это работает. 
5. [Ложная слепота](https://fantlab.ru/work134421) by Питер Уоттс - научная фантастика о том, как люди сталкиваются с ИИ
6. [The Ultimate GPT-4 Guide](https://hasantoxr.gumroad.com/l/gpt4) by [Hasan Toor](https://bio.link/hasantoxr) - Learn and Master everything about GPT-4 to enhance and level up your life. 
7. [Benchmarking](https://www.youtube.com/watch?v=ZnhFA-r_YvA) of GPU, а так же в практическом применении [RTX 2060 Vs GTX 1080Ti Deep Learning Benchmarks: Cheapest RTX card Vs Most Expensive GTX card](https://towardsdatascience.com/rtx-2060-vs-gtx-1080ti-in-deep-learning-gpu-benchmarks-cheapest-rtx-vs-most-expensive-gtx-card-cd47cd9931d2).
8. Техническая спецификация от [rtx-3070-3070ti](https://www.nvidia.com/en-eu/geforce/graphics-cards/30-series/rtx-3070-3070ti/), которая стоит примерно 94 000 динар

## Инструменты и программы

1. [chatGPT](https://chat.openai.com)
2. [DiffusionBee](https://diffusionbee.com) - DiffusionBee is the easiest way to generate AI art on your computer with Stable Diffusion. Completely free of charge. Runs offline. No limits. [Он на Гит](https://github.com/divamgupta/diffusionbee-stable-diffusion-ui). В него можно загружать разные модели [по инструкции](https://github.com/divamgupta/diffusionbee-stable-diffusion-ui/blob/master/DOCUMENTATION.md) из [huggingface](https://huggingface.co/models?other=stable-diffusion), в том числе и [midjourney-v4-diffusion](https://huggingface.co/flax/midjourney-v4-diffusion).
3. [How to Run Stable Diffusion Locally With a GUI on Windows](https://www.howtogeek.com/832491/how-to-run-stable-diffusion-locally-with-a-gui-on-windows/) - This fork also contains various optimizations that should allow it to run on PCs with less RAM, built-in upscaling and facial capabilities using GFPGAN, ESRGAN, RealESRGAN, and CodeFormer, and masking. Masking is a huge deal — it allows you to selectively apply the AI image generation to certain parts of the image without distorting other parts, a process typically called inpainting. Но стоит внимательно смотреть на системные требования.
4. [photofeeler](https://www.photofeeler.com) - программа, которая описывает фото параметрически, какое подойдет для резюме, а что - для службы знакомств
5. [whisper.cpp](https://github.com/ggerganov/whisper.cpp) - M1 версия [Whisper](https://github.com/openai/whisper/tree/main), программы по распознанию текста из речи
6. [llama.cpp](https://github.com/ggerganov/llama.cpp) - M1 версия [LLaMA](https://arxiv.org/abs/2302.13971): Open and Efficient Foundation Language Models. We introduce LLaMA, a collection of foundation language models ranging from 7B to 65B parameters. We train our models on trillions of tokens, and show that it is possible to train state-of-the-art models using publicly available datasets exclusively, without resorting to proprietary and inaccessible datasets. In particular, LLaMA-13B outperforms GPT-3 (175B) on most benchmarks, and LLaMA-65B is competitive with the best models, Chinchilla-70B and PaLM-540B. We release all our models to the research community. Очень важно внутрь положить оригинальные файлы LLaMA [по инструкции](https://github.com/facebookresearch/llama/issues/149)
7. [krisp](https://krisp.ai) - improves the productivity of online meetings with it’s AI-powered Voice Clarity and Meeting Assistant. Есть бесплатный тариф, но вообще [за деньги](https://krisp.ai/pricing/). Главный промо из двух частей: чистит звук, выступая виртуальным девайсом; умеет расшифровать текст, но только английский (вот и чего не wisper, который умеет и русский?)

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
