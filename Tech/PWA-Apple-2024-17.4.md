# Problem with PWA in Apple iOS 17.4-beta2/beta3

### What happened

Apple has indeed removed Progressive Web App (PWA) support from iOS in the EU with the release of iOS 17.4 beta 2. This change prevents PWAs from operating in a standalone mode, instead opening them as normal browser sessions. This move appears to be in response to the European Union's Digital Markets Act (DMA) antitrust legislation, which mandates that Apple allow alternative app stores and web browsers with their own engines on the iPhone. [1](https://www.perplexity.ai/search/6a34e8f6-362a-45de-9c8b-3fc09fb2ea42)

**It suggests the rule by account region**

### Is here something special for RU

> **В iOS 17.4 отключили поддержу PWA для пользователей из России и ЕС, почему это произошло?**
> 
> Внимание! Для пользователей из РФ PWA не отключали. Только для EC.  [3](https://habr.com/ru/news/792578/)

## Current state

for 17.4.beta2 on 12.02.2024
>We just re-tested this. For some unknown reason it seems to work now. Existing shortcuts still open wrong, but a newly added one works fine. Even opening an old shortcut and re-adding it to homesceen seems to work.
>
>Can anyone verify / are you experiencing the same?

for 17.4.beta3 on 13.02.2024
> Unfortunately it seems like it was just a glitch while Apple was releasing beta 3. At least it's now back to the same sad situation (for me at least).

## More information

1. [Has Apple removed pwa support from iOS in the EU?](https://www.perplexity.ai/search/6a34e8f6-362a-45de-9c8b-3fc09fb2ea42) on **Perplexity** summarize and follow the situation, contain link on other resourses, updatable last checked 14.02.2029
2. [Europa : PWA or A2HS in standalone no longer works](https://forums.developer.apple.com/forums/thread/745414) on **Apple's suppoer forum**, updatable last checked 14.02.2024
3. [В бете iOS 17.4 отключили PWA для Евросоюза](https://habr.com/ru/news/792578/) on **Habr RU** explains situation in Russia but from the single point of view, 09.02.2024
