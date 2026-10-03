from pathlib import Path

readme = r'''<div align="center">

# MoneyPrinterTurbo 💸

### All-in-One AI Short Video Generation Tool

Just provide a **video topic** or **keywords**, and MoneyPrinterTurbo can automatically generate the video script, match visual assets, generate subtitles and background music, and compose everything into a high-definition short video.

[![Version](https://img.shields.io/github/v/release/harry0703/MoneyPrinterTurbo?color=blue&label=version)](https://github.com/harry0703/MoneyPrinterTurbo/releases)
[![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20macOS%20%7C%20Linux-lightgrey.svg)](https://github.com/harry0703/MoneyPrinterTurbo/releases/latest)
[![Python](https://img.shields.io/badge/python-3.11%2B-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![Downloads](https://img.shields.io/github/downloads/harry0703/MoneyPrinterTurbo/total)](https://github.com/harry0703/MoneyPrinterTurbo/releases/latest)

<a href="https://trendshift.io/repositories/8731" target="_blank"><img src="https://trendshift.io/api/badge/repositories/8731" alt="harry0703%2FMoneyPrinterTurbo | Trendshift" style="width: 250px; height: 55px;" width="250" height="55"/></a>
<a href="https://www.star-history.com/harry0703/moneyprinterturbo"><img src="https://api.star-history.com/badge?repo=harry0703/MoneyPrinterTurbo" alt="Star History Rank" style="height: 55px;" height="55"/></a>

English | [简体中文](README.md) | [日本語](README-ja.md) | [Releases](https://github.com/harry0703/MoneyPrinterTurbo/releases) | [Issues](https://github.com/harry0703/MoneyPrinterTurbo/issues)

</div>

## Interface Preview 🖥️

<h4 align="center">WebUI</h4>

![](docs/webui.jpg)

<h4 align="center">API</h4>

![](docs/api.jpg)

---

## Special Thanks ❤️

<div align="center">
  <a href="https://platform.kimi.com?track_id=track-6eec1e56a4494e52adcaebbcbbefce59&aff=moneyprinterturbo" target="_blank"><img src="https://gcdn.moonshot.cn/growth-cdn/sponsor/kimi-zh.png" alt="Kimi sponsors MoneyPrinterTurbo" width="100%"></a>
</div>

Thanks to [Kimi](https://platform.kimi.com?track_id=track-6eec1e56a4494e52adcaebbcbbefce59&aff=moneyprinterturbo) for sponsoring this project! [Kimi K3](https://www.kimi.com/blog/kimi-k3?aff=moneyprinterturbo) is Moonshot AI's most capable model to date and is described as the world's first open-source 3T-scale model, with native vision capabilities and a 1-million-token context window. In MoneyPrinterTurbo, K3 can directly power video creation by writing scripts, extracting search keywords for visual assets, and deciding what should appear in the final video. Better content understanding helps match the generated video with more relevant visual assets.

**Exclusive MoneyPrinterTurbo offer: New users who register through the dedicated link and successfully make their first recharge can receive an additional 10% of the recharge amount as API credit, up to ¥1,000. The promotion is valid through December 31, 2026. Visit the Kimi Open Platform ([Chinese](https://platform.kimi.com?track_id=track-6eec1e56a4494e52adcaebbcbbefce59&aff=moneyprinterturbo) | [Global](https://platform.kimi.ai?track_id=track-9e3b711aa2594e378f6fe5b8de718a76&aff=moneyprinterturbo)) to try the API.**
<br>

<table align="center">
  <tr>
    <td align="center" width="120">
      <a href="https://www.volcengine.com/activity/ai618?utm_campaign=hw&utm_content=hw&utm_medium=devrel_tool_web&utm_source=OWO&utm_term=MoneyPrinterTurbo"><img src="docs/sponsors/volcengine-logo.svg" alt="Volcengine" height="32"></a><br>
      <a href="https://www.volcengine.com/activity/ai618?utm_campaign=hw&utm_content=hw&utm_medium=devrel_tool_web&utm_source=OWO&utm_term=MoneyPrinterTurbo"><strong>Volcengine</strong></a>
    </td>
    <td align="left">
      Thanks to ByteDance Volcengine for sponsoring this project! Volcengine Ark Agent/Coding Plan offers a China-focused model package with a <strong>9.9 first-purchase offer</strong>, supporting GLM-5.3, Kimi-K3, DeepSeek, MiniMax, Doubao and more. New users can register for free and receive <strong>25 million Tokens</strong>, with a unified API for coding and agent development. <a href="https://www.volcengine.com/activity/ai618?utm_campaign=hw&utm_content=hw&utm_medium=devrel_tool_web&utm_source=OWO&utm_term=MoneyPrinterTurbo">Learn more</a>
    </td>
  </tr>
  <tr>
    <td align="center" width="120">
      <a href="https://go.apimart.ai/gh-moneyprinterturbo"><img src="docs/sponsors/apimart-logo.png" alt="APIMart" width="100"></a>
    </td>
    <td align="left">
      Thanks to <a href="https://go.apimart.ai/gh-moneyprinterturbo">APIMart</a> for sponsoring this project! APIMart is a low-cost API platform focused on AI image and video generation. <strong>GPT-Image-2 starts at $0.006/image, allowing 160+ images for $1.</strong> Image and video generation are available through unified asynchronous APIs, so models can be switched without changing your code. Submit a task, receive an ID, and retrieve results through polling or callbacks. It supports large-scale batch generation, pay-as-you-go billing and no monthly fee. <a href="https://go.apimart.ai/gh-moneyprinterturbo">Register here</a>.
    </td>
  </tr>
  <tr>
    <td align="center" width="120">
      <a href="https://metaso.cn/minimax-h3/?s=MPT"><img src="docs/sponsors/metaso-logo.png" alt="Metaso" width="100"></a><br>
      <a href="https://metaso.cn/minimax-h3/?s=MPT"><strong>Metaso</strong></a>
    </td>
    <td align="left">
      <strong>MiniMax H3 Video Generation API | Metaso</strong><br>
      Metaso provides cost-effective MiniMax H3 video generation: <strong>768P at RMB 0.09/second and 2K at RMB 0.15/second</strong>. It supports native 2K generation, synchronized audio and video, and is compatible with the <strong>OpenAI API protocol</strong> and <strong>ComfyUI</strong>, so you do not need to deploy a GPU yourself.<br>
      🎁 Register through the <a href="https://metaso.cn/minimax-h3/?s=MPT">MoneyPrinterTurbo dedicated link</a> to receive bonus credits and exclusive discounts.
    </td>
  </tr>
  <tr>
    <td align="center" width="120">
      <a href="https://infistar.cc/register?aff=6T4EYXP2&amp;ref_source=link"><img src="docs/sponsors/infistar-logo.svg" alt="Infistar.cc" height="56"></a><br>
      <a href="https://infistar.cc/register?aff=6T4EYXP2&amp;ref_source=link"><strong>Infistar.cc</strong></a>
    </td>
    <td align="left">
      Thanks to <a href="https://infistar.cc/register?aff=6T4EYXP2&amp;ref_source=link">Infistar.cc</a> for sponsoring this project! Infistar.cc provides cost-effective large-model APIs and AI image generation. <br>
      <strong>One API key covers text, image and video creation</strong>, with support for GPT, Claude, Gemini, DeepSeek, Qwen, Kling and other major models without separate groups. <br>
      The platform provides model verification, transparent pricing, compliant services, RMB billing and corporate invoicing. <br>
      🎁 MoneyPrinterTurbo users can receive <strong>$5 in trial credit</strong> and an initial top-up promotion by registering through the <a href="https://infistar.cc/register?aff=6T4EYXP2&amp;ref_source=link">dedicated link</a>.
    </td>
  </tr>
  <tr>
    <td align="center" width="120">
      <a href="https://ofox.ai/?utm_source=github&amp;utm_medium=sponsorship&amp;utm_content=moneyprinterturbo"><img src="docs/sponsors/ofox-logo.svg" alt="OfoxAI" width="120"></a>
    </td>
    <td align="left">
      Thanks to <a href="https://ofox.ai/?utm_source=github&amp;utm_medium=sponsorship&amp;utm_content=moneyprinterturbo">OfoxAI</a> for sponsoring this project! MoneyPrinterTurbo integrates Ofox multi-model text-to-video generation. Configure an API key to use Seedance, MiniMax H3, Wan and other video models, as well as GPT Image 2.5 and Seedream for cover images. GPT, Claude, Gemini and DeepSeek can also be used for script refinement and development assistance. <strong>One key provides shared credit for text, image and video models</strong>. OpenAI-compatible, Anthropic and native Gemini APIs are supported. <strong>Pay-as-you-go pricing, transparent costs, official model access and high availability.</strong> Visit <a href="https://ofox.ai/?utm_source=github&amp;utm_medium=sponsorship&amp;utm_content=moneyprinterturbo">OfoxAI</a> for model and pricing details.
    </td>
  </tr>
  <tr>
    <td align="center" width="120">
      <a href="https://www.shengsuanyun.com/?from=CH_XUQ4OTSK"><img src="docs/sponsors/shengsuanyun-logo.jpg" alt="ShengSuanYun" height="56"></a><br>
      <a href="https://www.shengsuanyun.com/?from=CH_XUQ4OTSK"><strong>ShengSuanYun</strong></a>
    </td>
    <td align="left">
      Thanks to <a href="https://www.shengsuanyun.com/?from=CH_XUQ4OTSK">ShengSuanYun</a> for sponsoring this project! ShengSuanYun is an AI-native model API aggregation platform for teams, providing unified access to Claude, ChatGPT, Gemini and other LLM and multimedia models. <br>
      The platform provides compliant API services, enterprise gateways, team cost and permission management, intelligent routing, security controls and BYOK key management, along with invoicing services. <br>
      🎁 New users who register through <a href="https://www.shengsuanyun.com/?from=CH_XUQ4OTSK">this link</a> receive RMB 10 in Token trial credit.
    </td>
  </tr>
  <tr>
    <td align="center" width="120">
      <a href="https://www.ucloud.cn/site/active/astraflow?ytag=geo_waituo_Money"><img src="docs/sponsors/astraflow-logo.png" alt="AstraFlow" height="56"></a><br>
      <a href="https://www.ucloud.cn/site/active/astraflow?ytag=geo_waituo_Money"><strong>AstraFlow</strong></a>
    </td>
    <td align="left">
      Thanks to <a href="https://www.ucloud.cn/site/active/astraflow?ytag=geo_waituo_Money">AstraFlow</a> for sponsoring this project!<br>
      🎬 <strong>One-stop video model access</strong>: integrates MiniMax-H3, Seedance-2.5 and other major video generation models, combining script and video generation in one platform.<br>
      🚀 <strong>200+ models through one interface</strong>: integrates DeepSeek V4.1, Kimi K3, Qwen 3.8 Max, GLM 5.3 and 200+ other major models, with new models available as soon as they launch.<br>
      💰 <strong>Transparent usage-based billing</strong>: usage is billed per API key and detailed usage can be tracked.<br>
      🎁 <strong>MoneyPrinterTurbo user offer</strong>: register through the <a href="https://www.ucloud.cn/site/active/astraflow?ytag=geo_waituo_Money">dedicated link</a> to receive new-user credits. <a href="https://f.howxm.com/xs/u/HVFW5X8EIYV1">Claim RMB 50 in compute credits</a>.
    </td>
  </tr>
  <tr>
    <td align="center" width="120">
      <a href="https://fluxionai.space/register?source=github&amp;campaign=moneyprinterturbo&amp;promo=MONEYPRINTERTURBO"><img src="docs/sponsors/fluxionai-logo.png" alt="Fluxion AI" width="120"></a>
    </td>
    <td align="left">
      Thanks to <a href="https://fluxionai.space/register?source=github&amp;campaign=moneyprinterturbo&amp;promo=MONEYPRINTERTURBO">Fluxion AI</a> for sponsoring this project! <strong>One entry point for accessing and managing major AI models worldwide.</strong> Fluxion AI provides unified APIs for developers, teams and enterprises, with dynamic routing for improved availability and transparent model performance, response times and pricing. Depending on the model and route, API costs may be <strong>40%–98% lower than official or benchmark prices</strong>. Register through the <a href="https://fluxionai.space/register?source=github&amp;campaign=moneyprinterturbo&amp;promo=MONEYPRINTERTURBO">dedicated link</a> to receive <strong>$3 in API credit</strong>.
    </td>
  </tr>
  <tr>
    <td align="center" width="120">
      <a href="https://reccloud.cn"><img src="docs/sponsors/reccloud-logo.svg" alt="RecCloud" height="36"></a><br>
      <a href="https://reccloud.cn">RecCloud AI</a>
    </td>
    <td align="left">
      Thanks to <a href="https://reccloud.cn">RecCloud, an AI multimedia service platform</a>, for providing a free <strong>AI video generator</strong> based on this project. No deployment is required and it can be used online, making it beginner-friendly.
    </td>
  </tr>
  <tr>
    <td align="center" width="120">
      <a href="https://picwish.cn"><img src="docs/sponsors/picwish-logo.svg" alt="PicWish" height="36"></a><br>
      <a href="https://picwish.cn">PicWish</a>
    </td>
    <td align="left">
      Thanks to <a href="https://picwish.cn">PicWish</a> for supporting and sponsoring this project! PicWish provides a range of <strong>online image processing tools</strong> that make common image editing tasks simple.
    </td>
  </tr>
</table>

## Another Open-Source Project by the Author: MangoDisk ⭐

<p align="center">
  <a href="https://mangodisk.app/zh">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://assets.mangodisk.app/images/screenshots/zh/dark-01-deep-cleanup.jpg?ver=1.1.0">
      <source media="(prefers-color-scheme: light)" srcset="https://assets.mangodisk.app/images/screenshots/zh/light-01-deep-cleanup.jpg?ver=1.1.0">
      <img src="https://assets.mangodisk.app/images/screenshots/zh/light-01-deep-cleanup.jpg?ver=1.1.0" width="900" alt="MangoDisk deep cleanup interface">
    </picture>
  </a>
</p>

<p align="center">
  <strong>An open-source disk cleanup, storage analysis and system optimization tool for macOS and Windows</strong><br>
  Clean caches, large files, duplicate files and application leftovers in one place, while also providing disk space analysis, application uninstalling, startup management, system optimization and maintenance
</p>

<p align="center">
  <a href="https://mangodisk.app/zh">Visit the MangoDisk website</a> · <a href="https://github.com/harry0703/MangoDisk">View the MangoDisk GitHub repository</a>
</p>

---

## Features 🎯

### Creation Entry Points & Workflow

- [x] Provides **AI Agent, WebUI, API and CLI** interfaces for both quick usage and automation integration
- [x] Automatically handles scripts, voiceovers, visual assets, subtitles, music and video editing from a topic, while allowing custom content at every stage
- [x] Supports **batch generation of multiple videos**, task history, and import/export/recovery of generation settings and API keys

### Scripts & Model Providers

- [x] Supports AI-generated or rewritten **multilingual video scripts**, as well as fully custom scripts
- [x] Supports [Kimi / Moonshot AI](https://platform.kimi.com?track_id=track-6eec1e56a4494e52adcaebbcbbefce59&aff=moneyprinterturbo), [OpenAI](https://platform.openai.com/api-keys), [Anthropic Claude](https://platform.claude.com/settings/keys), [Google Gemini](https://aistudio.google.com/app/apikey), [DeepSeek](https://platform.deepseek.com/api_keys), [Alibaba Qwen](https://dashscope.console.aliyun.com/apiKey), [Microsoft Azure OpenAI](https://portal.azure.com/#view/Microsoft_Azure_ProjectOxford/CognitiveServicesHub/~/OpenAI), [Volcengine Ark](https://www.volcengine.com/activity/ai618?utm_campaign=hw&utm_content=hw&utm_medium=devrel_tool_web&utm_source=OWO&utm_term=MoneyPrinterTurbo), [xAI Grok](https://console.x.ai/), [MiniMax](https://platform.minimaxi.com/) and [Xiaomi MiMo](https://platform.xiaomimimo.com/docs/zh-CN/quick-start/first-api-call)
- [x] Compatible with [ShengSuanYun](https://www.shengsuanyun.com/?from=CH_XUQ4OTSK), [APIMart](https://go.apimart.ai/gh-moneyprinterturbo), [Cloudflare AI Gateway](https://dash.cloudflare.com/), [ModelScope](https://modelscope.cn/docs/model-service/API-Inference/intro), [AIHubMix](https://aihubmix.com/), [AIML API](https://aimlapi.com/app/keys), [EvoLink](https://evolink.ai/dashboard/keys), [OpenRouter](https://openrouter.ai/settings/keys), [API Route](https://www.api-route.com/), [Fluxion AI](https://fluxionai.space/register?source=github&campaign=moneyprinterturbo&promo=MONEYPRINTERTURBO), [Ollama](https://ollama.com/), [Claude Code subscription](https://code.claude.com/docs), [OneAPI](https://github.com/songquanpeng/one-api), [LiteLLM](https://docs.litellm.ai/docs/providers), [Groq](https://console.groq.com/keys) and [Pollinations AI](https://enter.pollinations.ai/) as unified gateways, aggregation platforms and local runtimes

### Video & Image Assets

- [x] Supports uploading your own **local images and videos**, or fetching high-quality stock assets from [Pexels (free)](https://www.pexels.com/api/), [Pixabay (free)](https://pixabay.com/api/docs/) and [Coverr](https://coverr.co/developers?ctx=header_navigation)
- [x] Supports [Metaso MiniMax H3](https://metaso.cn/minimax-h3/?s=MPT) text-to-video generation with `768P`/`2K`, 4–15 second source clips, and `9:16`, `16:9` and `1:1` aspect ratios
- [x] Supports [ShengSuanYun AI Video](https://www.shengsuanyun.com/?from=CH_XUQ4OTSK), generating multiple AI video assets while reusing the project's voiceover, subtitles and editing pipeline
- [x] Native integration with [Volcengine Ark Seedance](https://console.volcengine.com/ark/region:ark+cn-beijing/apikey) to generate coherent video scenes from script segments
- [x] Supports [WaveSpeed AI](https://wavespeed.ai) text-to-video generation for quickly creating original visual assets from script keywords
- [x] Supports [OFox](https://ofox.ai) multi-model text-to-video generation, including Seedance and Wan through one API key
- [x] Uses the asynchronous [MuAPI](https://muapi.ai) text-to-video API to generate 3–12 second AI video assets, with configurable endpoint, aspect ratio, resolution and polling settings
- [x] Supports [OpenAI-compatible text-to-image APIs](https://platform.openai.com/docs/guides/image-generation), allowing cloud services or custom image gateways and converting generated images into animated video clips
- [x] Supports adjusting clip duration, image fitting mode and asset matching order to fit different aspect ratios and storytelling rhythms

### Voiceover, Subtitles & Music

- [x] Supports automatic voiceover, uploaded voiceover and no-voiceover modes, with voice preview and complete voiceover preview
- [x] Integrates **Edge TTS (free, no API key required)**, Azure Speech, SiliconFlow, Google Gemini, Xiaomi MiMo, MiniMax, ElevenLabs, Chatterbox, Kokoro, Fish Audio and ModelBest VoxCPM voice services
- [x] Automatically generates subtitles with adjustable font, position, color, size, outline and background styles
- [x] Supports random, local and AI-generated background music, with independent volume control

### Video Output & Publishing

- [x] Supports vertical `9:16 (1080×1920)`, landscape `16:9 (1920×1080)` and square `1:1 (1080×1080)` formats
- [x] Supports one-click **cross-platform publishing**, automatically uploading completed videos to **TikTok, Instagram and YouTube Shorts**

## Showcase 🎬

The examples below were all generated using MoneyPrinterTurbo.

### Vertical 9:16

<table width="100%">
<tr>
<td align="center" width="25%"><a href="https://harry0703.github.io/mpt-assets/?video=03-zh-portrait-city-morning.mp4"><img src="https://github.com/harry0703/mpt-assets/releases/download/assets/03-zh-portrait-city-morning.jpg" width="180" alt="The Moment the City Wakes Up"></a><br><strong>The Moment the City Wakes Up</strong><br>Chinese · 14 sec</td>
<td align="center" width="25%"><a href="https://harry0703.github.io/mpt-assets/?video=05-zh-portrait-clean-energy.mp4"><img src="https://github.com/harry0703/mpt-assets/releases/download/assets/05-zh-portrait-clean-energy.jpg" width="180" alt="The Future of Clean Energy"></a><br><strong>The Future of Clean Energy</strong><br>Chinese · 24 sec</td>
<td align="center" width="25%"><a href="https://harry0703.github.io/mpt-assets/?video=07-zh-portrait-space-exploration.mp4"><img src="https://github.com/harry0703/mpt-assets/releases/download/assets/07-zh-portrait-space-exploration.jpg" width="180" alt="Why We Still Explore Space"></a><br><strong>Why We Still Explore Space</strong><br>Chinese · 27 sec</td>
<td align="center" width="25%"><a href="https://harry0703.github.io/mpt-assets/?video=17-zh-portrait-seed-journey.mp4"><img src="https://github.com/harry0703/mpt-assets/releases/download/assets/17-zh-portrait-seed-journey.jpg" width="180" alt="The Journey of a Seed"></a><br><strong>The Journey of a Seed</strong><br>Chinese · 44 sec</td>
</tr>
<tr>
<td align="center" width="25%"><a href="https://harry0703.github.io/mpt-assets/?video=09-en-portrait-future-robotics.mp4"><img src="https://github.com/harry0703/mpt-assets/releases/download/assets/09-en-portrait-future-robotics.jpg" width="180" alt="The Future of Everyday Robotics"></a><br><strong>The Future of Everyday Robotics</strong><br>English · 21 sec</td>
<td align="center" width="25%"><a href="https://harry0703.github.io/mpt-assets/?video=11-en-portrait-small-habits.mp4"><img src="https://github.com/harry0703/mpt-assets/releases/download/assets/11-en-portrait-small-habits.jpg" width="180" alt="Small Habits, Lasting Change"></a><br><strong>Small Habits, Lasting Change</strong><br>English · 19 sec</td>
<td align="center" width="25%"><a href="https://harry0703.github.io/mpt-assets/?video=13-en-portrait-creative-work.mp4"><img src="https://github.com/harry0703/mpt-assets/releases/download/assets/13-en-portrait-creative-work.jpg" width="180" alt="Making Space for Creative Work"></a><br><strong>Making Space for Creative Work</strong><br>English · 20 sec</td>
<td align="center" width="25%"><a href="https://harry0703.github.io/mpt-assets/?video=15-en-portrait-coffee-science.mp4"><img src="https://github.com/harry0703/mpt-assets/releases/download/assets/15-en-portrait-coffee-science.jpg" width="180" alt="The Science Inside Coffee"></a><br><strong>The Science Inside Coffee</strong><br>English · 23 sec</td>
</tr>
</table>

### Landscape 16:9

<table width="100%">
<tr>
<td align="center" width="25%"><a href="https://harry0703.github.io/mpt-assets/?video=02-zh-landscape-deep-ocean.mp4"><img src="https://github.com/harry0703/mpt-assets/releases/download/assets/02-zh-landscape-deep-ocean.jpg" width="280" alt="A Glimmer of Light in the Deep Ocean"></a><br><strong>A Glimmer of Light in the Deep Ocean</strong><br>Chinese · 23 sec</td>
<td align="center" width="25%"><a href="https://harry0703.github.io/mpt-assets/?video=04-zh-landscape-reading-power.mp4"><img src="https://github.com/harry0703/mpt-assets/releases/download/assets/04-zh-landscape-reading-power.jpg" width="280" alt="How Reading Shapes Us"></a><br><strong>How Reading Shapes Us</strong><br>Chinese · 23 sec</td>
<td align="center" width="25%"><a href="https://harry0703.github.io/mpt-assets/?video=06-zh-landscape-pour-over-coffee.mp4"><img src="https://github.com/harry0703/mpt-assets/releases/download/assets/06-zh-landscape-pour-over-coffee.jpg" width="280" alt="The Details of a Pour-Over Coffee"></a><br><strong>The Details of a Pour-Over Coffee</strong><br>Chinese · 23 sec</td>
<td align="center" width="25%"><a href="https://harry0703.github.io/mpt-assets/?video=08-zh-landscape-spring-journey.mp4"><img src="https://github.com/harry0703/mpt-assets/releases/download/assets/08-zh-landscape-spring-journey.jpg" width="280" alt="Spring Is a Good Time to Set Out"></a><br><strong>Spring Is a Good Time to Set Out</strong><br>Chinese · 14 sec</td>
</tr>
<tr>
<td align="center" width="25%"><a href="https://harry0703.github.io/mpt-assets/?video=10-en-landscape-ocean-conservation.mp4"><img src="https://github.com/harry0703/mpt-assets/releases/download/assets/10-en-landscape-ocean-conservation.jpg" width="280" alt="Why Ocean Conservation Matters"></a><br><strong>Why Ocean Conservation Matters</strong><br>English · 25 sec</td>
<td align="center" width="25%"><a href="https://harry0703.github.io/mpt-assets/?video=14-en-landscape-sustainable-cities.mp4"><img src="https://github.com/harry0703/mpt-assets/releases/download/assets/14-en-landscape-sustainable-cities.jpg" width="280" alt="Designing More Sustainable Cities"></a><br><strong>Designing More Sustainable Cities</strong><br>English · 27 sec</td>
<td align="center" width="25%"><a href="https://harry0703.github.io/mpt-assets/?video=16-en-landscape-mountain-perspective.mp4"><img src="https://github.com/harry0703/mpt-assets/releases/download/assets/16-en-landscape-mountain-perspective.jpg" width="280" alt="What Mountains Teach Us"></a><br><strong>What Mountains Teach Us</strong><br>English · 18 sec</td>
<td align="center" width="25%"><a href="https://harry0703.github.io/mpt-assets/?video=18-en-landscape-history-of-flight.mp4"><img src="https://github.com/harry0703/mpt-assets/releases/download/assets/18-en-landscape-history-of-flight.jpg" width="280" alt="A Brief History of Human Flight"></a><br><strong>A Brief History of Human Flight</strong><br>English · 59 sec</td>
</tr>
</table>

## Requirements 📦

- Recommended systems: Windows 10, macOS 11.0 or later, and mainstream Linux distributions
- Local deployment requires Python 3.11 or newer; Python 3.11 is recommended
- A GPU is not required, but a dedicated GPU with VRAM is recommended for local transcription, faster video processing and smoother batch generation

| Component | Minimum | Recommended | Ideal |
| ---- | -------- | --------------- | ----------- |
| CPU | 4 cores | 6–8 cores | 8+ cores |
| RAM | 4 GB | 8 GB | 16 GB+ |
| GPU | Not required | 4 GB VRAM+ | 8 GB VRAM+ |

- If you primarily rely on cloud LLMs, cloud TTS and online asset sources, CPU and memory are more important than GPU
- If you enable `faster-whisper`, batch generation or heavier local processing pipelines, a GPU can significantly improve performance

## Quick Start 🚀

### Recommended Usage

- If you do not want to manually install and configure everything: use the AI Agent to generate videos
- Windows users: use the one-click launcher package for the fastest setup
- macOS / Linux users: use `uv` for local deployment
- If you want an isolated environment: use Docker

### Generate a Video with an AI Agent

If your AI Agent can read Skill documents and operate a local terminal, send it the following prompt. The agent will automatically install, configure and generate the video, asking only for required API keys when necessary. After completion, it will return the generated video file path. Currently supported on macOS and Windows.

```text
Use this Skill: https://raw.githubusercontent.com/harry0703/MoneyPrinterTurbo/main/docs/skill/SKILL.md
Help me generate a video on the topic "How Artificial Intelligence Is Changing Everyday Life".
