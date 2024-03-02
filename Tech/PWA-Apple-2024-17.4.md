# Problem with PWA in Apple iOS 17.4 (starts from beta2)

Resume: the return of the existing functionality for Home Screen web apps with the availability of iOS 17.4 in early March

## Latest update (yet)

> Previously, Apple announced plans to remove the Home Screen web apps capability in the EU as part of our efforts to comply with the DMA. The need to remove the capability was informed by the complex security and privacy concerns associated with web apps to support alternative browser engines that would require building a new integration architecture that does not currently exist in iOS.
>
> We have received **requests to continue to offer support for Home Screen web apps in iOS**, therefore we will continue to offer the existing Home Screen web apps capability in the EU. This support means **Home Screen web apps continue to be built directly on WebKit** and its security architecture, and align with the security and privacy model for native apps on iOS.
>
> Developers and users who may have been impacted by the removal of Home Screen web apps in the beta release of iOS in the EU can expect the return of the existing functionality for Home Screen web apps with the availability of iOS 17.4 in early March.

_[Update on apps distributed in the European Union](https://developer.apple.com/support/dma-and-apps-in-the-eu/#ntfqa) by Apple found by [Apple says iOS 17.4 won’t remove Home Screen web apps in the EU after all](https://9to5mac.com/2024/03/01/apple-home-screen-web-apps-ios-17-eu/) on 1st March 2024_

> To me, this is an example of the vagueness of the Digital Markets Act. Reading between the lines, it sounds like Apple thought it couldn’t offer WebKit-powered Home Screen apps in the European Union because of the DMA’s guidelines on browser equality.
(c) Chance Miller in [Apple says iOS 17.4 won’t remove Home Screen web apps in the EU after all](https://9to5mac.com/2024/03/01/apple-home-screen-web-apps-ios-17-eu/)

**Why don't users in the EU have access to Home Screen web apps?** [4](https://developer.apple.com/support/dma-and-apps-in-the-eu)

> To comply with the Digital Markets Act, Apple has done an enormous amount of engineering work to add new functionality and capabilities for developers and users in the European Union — including more than 600 new APIs and a wide range of developer tools.
>
> The iOS system has traditionally provided support for Home Screen web apps by building directly on WebKit and its security architecture. That integration means Home Screen web apps are managed to align with the security and privacy model for native apps on iOS, including isolation of storage and enforcement of system prompts to access privacy impacting capabilities on a per-site basis.
>
> Without this type of isolation and enforcement, malicious web apps could read data from other web apps and recapture their permissions to gain access to a user’s camera, microphone or location without a user’s consent. Browsers also could install web apps on the system without a user’s awareness and consent. Addressing the complex security and privacy concerns associated with web apps using alternative browser engines would require building an entirely new integration architecture that does not currently exist in iOS and was not practical to undertake given the other demands of the DMA and the very low user adoption of Home Screen web apps. And so, to comply with the DMA’s requirements, we had to remove the Home Screen web apps feature in the EU.
>
> EU users will be able to continue accessing websites directly from their Home Screen through a bookmark with minimal impact to their functionality. We expect this change to affect a small number of users. Still, we regret any impact this change — that was made as part of the work to comply with the DMA — may have on developers of Home Screen web apps and our users.


### What happened

Apple has indeed removed Progressive Web App (PWA) support from iOS in the EU with the release of iOS 17.4 beta 2. This change prevents PWAs from operating in a standalone mode, instead opening them as normal browser sessions. This move appears to be in response to the European Union's Digital Markets Act (DMA) antitrust legislation, which mandates that Apple allow alternative app stores and web browsers with their own engines on the iPhone. [1](https://www.perplexity.ai/search/6a34e8f6-362a-45de-9c8b-3fc09fb2ea42)

**It suggests the rule by account region**

The changes are available for developers who distribute apps in any of the **27 EU member countries and only apply to apps available and distributed to users in the EU**. For existing developers who want nothing to change for them — from how the App Store works currently and in the rest of the world — no action is needed, and they can continue to distribute their apps only on the App Store and use its private and secure In-App Purchase system. [4](https://developer.apple.com/support/dma-and-apps-in-the-eu)

> Austria, Belgium, Bulgaria, Croatia, Cyprus, Czechia, Denmark, Estonia, Finland, France, Germany, Greece, Hungary, Ireland, Italy, Latvia, Lithuania, Luxembourg, Malta, Netherlands, Poland, Portugal, Romania, Slovakia, Slovenia, Spain, Sweden


### Is here something special for RU

> **В iOS 17.4 отключили поддержу PWA для пользователей из России и ЕС, почему это произошло?**
> 
> Внимание! Для пользователей из РФ PWA не отключали. Только для EC.  [3](https://habr.com/ru/news/792578/)

## Current state

Resume: the return of the existing functionality for Home Screen web apps with the availability of iOS 17.4 in early March [5]

for 17.4 included [in release notes](https://developer.apple.com/support/dma-and-apps-in-the-eu#dev-qa)

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
4. [Update on apps distributed in the European Union](https://developer.apple.com/support/dma-and-apps-in-the-eu) by Apple
5. [Apple says iOS 17.4 won’t remove Home Screen web apps in the EU after all](https://9to5mac.com/2024/03/01/apple-home-screen-web-apps-ios-17-eu/), 9to5mac, 01.march.24
