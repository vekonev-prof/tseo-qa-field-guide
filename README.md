# Technical SEO Field Guide for QA (TSEO Big Guideline)

**RU-гайд для QA-инженеров** · Public edition — no client data, no internal tooling

## О гайде
Полевой чек-лист технического SEO-аудита для QA-инженеров, которые тестируют сайты и отвечают не только за функциональность, но и за индексацию, скорость и видимость сайта в поиске.

Собран на основе 40+ технических SEO-аудитов production-сайтов (американский рынок, лидогенерирующие сайты, стек Webflow/WordPress + Cloudflare). Публичная редакция: внутренние названия процессов, аккаунты и клиентские данные удалены.

## Что внутри (`tseo-field-guide-public.md`)
- **0_Simplified** — экспресс-аудит: 10 самых критичных проверок
- **1_Basic** — полный аудит: robots.txt, meta robots / X-Robots-Tag, AI-краулеры (GPTBot и др.), sitemap.xml, canonical, www/http-редиректы, GSC (индексация, ошибки, crawl stats), Schema/JSON-LD, структура URL, page depth, текстовая версия страницы, лидогенерящие каналы
- **2_Codes** — коды ответов: 3xx/4xx/5xx, soft-404, цепочки редиректов, сверка миграции по карте редиректов
- **3_Performance** — Core Web Vitals + PageSpeed Insights (пороги, приоритет полевых данных), диагностика LCP/srcset, приёмы DevTools
- **4_Content** — тайтлы и дескрипшены, перелинковка, alt/вес/форматы картинок, srcset, H-структура, дубли, OG-теги, кастомные поиски кириллицы и Lorem Ipsum
- **5_Multilingual** — hreflang, x-default, return links, редиректы языковых версий
- **6_Misc** — crawl budget, JS-рендеринг, блокировки стран
- **7_UX** — меню и навигация, формы, breadcrumbs, iframe, пагинация/related
- **8_Situational** — каннибализация запросов (GSC), MS Clarity, marTech-сервисы, доступы

Формат каждой проверки: **«Что и зачем → Что делать → Инструменты»**, с чёткой границей ответственности (что находит и чинит QA, а что решает SEO).

## Инструменты
Screaming Frog, Google Search Console, PageSpeed Insights, Rich Results Test, DevTools, Link Redirect Trace, metatags.io, MS Clarity, DNSChecker.

## Как использовать
1. Прогоняйте по чек-листу перед релизом и на регулярных проверках LIVE-сайтов.
2. Пункты, помеченные `→ SEO`, — спорные/стратегические: фиксируйте находку и передавайте SEO-специалисту, не решайте единолично.
3. Часть проверок автоматизирована моим AI QA-агентом (Claude Code + Playwright) — см. закреплённые репозитории профиля.

## Автор
**Владислав Конев** — QA Engineer (web + technical SEO QA)
[LinkedIn](https://www.linkedin.com/in/vekonevprof/) · [GitHub](https://github.com/vekonev-prof)

> Disclaimer: материал носит образовательный характер, основан на публичной документации Google и личном опыте автора; не является официальной документацией Google.