# Jintat Industrial Website V3 Master Prompt for Codex

This document is the master instruction file for redesigning the Jintat Industrial website.

Repository: `chindynasty123-cmd/jintat.github.io`

Primary file to modify: `index.html`

Website purpose: Build trust with overseas buyers looking for a Taiwan CNC precision machining partner.

---

## 0. Critical Instructions

This website is fully bilingual.

Every visible content change MUST include both:

- English
- Traditional Chinese

Use the existing `data-i18n` language switch system.

Do NOT create English-only content.
Do NOT create Chinese-only content.
Do NOT remove or break the current language switch JavaScript.

Preserve all existing business-critical information:

- Company name: Jintat Industrial Co., Ltd.
- Chinese name: 瑨達工業有限公司
- Email: `jintat@jintat.com`
- Mobile: `+886-918-853-297`
- TEL: `+886-4-8367999`
- Established background: 2005
- ISO 9001 positioning
- CNC turning / milling capability
- Mitutoyo CMM
- Keyence measurement
- Prototype and low-volume support
- High-mix low-volume support
- Overseas RFQ support

Do NOT remove:

- SEO meta tags
- canonical tag
- Open Graph tags
- Twitter card tags
- JSON-LD structured data
- FAQ schema
- mailto RFQ links
- existing image assets
- lightbox function
- language switch function

You may rewrite visual layout, CSS, section order and visible copy, but do not destroy SEO structure or business data.

---

## 1. Design Goal

Redesign the site from a crowded dark-blue technical landing page into a premium international CNC machining brand website.

The result should feel like:

- professional
- precise
- industrial
- trustworthy
- clean
- international
- calm
- buyer-friendly

Avoid:

- cheap template look
- overly bright SaaS blue gradient
- crowded cards
- too many badges at once
- heavy text blocks
- random visual hierarchy
- stock-photo feeling
- cartoon or AI-generated visual style

The site should make an overseas buyer feel:

> This is a real Taiwan precision machining company. They are not the biggest, but they look reliable, organized, responsive and capable of handling drawings professionally.

---

## 2. Visual Direction

Use a black / graphite / metallic industrial look.

Suggested colors:

```css
:root {
  --bg: #080b10;
  --bg-soft: #0f141c;
  --panel: rgba(18, 24, 33, 0.82);
  --panel-strong: rgba(22, 29, 39, 0.94);
  --text: #f4f7fb;
  --muted: #aeb8c7;
  --muted-2: #7d8898;
  --line: rgba(255,255,255,.10);
  --line-strong: rgba(255,255,255,.18);
  --metal: #d8dee8;
  --accent: #7fb5ff;
  --accent-soft: rgba(127,181,255,.16);
  --gold: #d7b46a;
  --shadow: 0 24px 80px rgba(0,0,0,.48);
  --radius: 20px;
  --radius-lg: 28px;
}
```

Guidelines:

- Use black and graphite as the main base.
- Use white and metallic silver for typography.
- Use blue only as a subtle precision/engineering highlight.
- Use gold only very sparingly if it helps premium feel.
- Avoid large bright gradients.
- Use subtle radial glows, thin lines and metallic borders.
- Use generous spacing.
- Make the layout breathe.

---

## 3. Typography and Spacing

Use system fonts unless a safe web font is already available.

Typography rules:

- H1 desktop: 56px max, 44px minimum depending layout
- H1 mobile: 32px to 38px
- H2 desktop: 34px to 42px
- H2 mobile: 26px to 32px
- Body text: 15px to 17px
- Line-height: 1.55 to 1.75
- Avoid long paragraphs over 3 lines on desktop when possible

Spacing rules:

- Section vertical padding desktop: 84px to 110px
- Section vertical padding mobile: 56px to 72px
- Card padding desktop: 28px to 36px
- Card padding mobile: 20px to 24px
- Grid gap: 18px to 28px

The site should feel premium through spacing, not decoration.

---

## 4. Navigation

Simplify the desktop navigation.

Desktop nav items:

English:
- About
- Capabilities
- Industries
- Quality
- Contact

Traditional Chinese:
- 關於瑨達
- 加工能力
- 應用產業
- 品質管理
- 聯絡詢價

Keep:

- EN / 中文 switch
- Send Drawing CTA button

Navigation style:

- Sticky top bar
- Dark translucent background
- Subtle blur
- Thin bottom border
- Logo on left
- Navigation centered or right aligned
- CTA on far right

Mobile navigation:

- Use hamburger menu
- Hide desktop nav links on mobile
- Full-screen or slide-down dark menu
- Menu must include all nav links, language buttons and Send Drawing CTA
- Clicking a menu link closes the menu
- ESC key closes menu if simple to implement
- Prevent horizontal scroll

---

## 5. Recommended Page Structure

Reorder the page into this structure:

1. Hero
2. Trust Bar / Why Jintat
3. Capabilities
4. Industries
5. Proof of Capability
6. Machine & Inspection Equipment
7. Quality & Documentation
8. RFQ / Contact
9. Buyer Questions / FAQ
10. Footer

Do not let FAQ or SEO-style content appear too high on the page.

---

## 6. Hero Section

The Hero must be clean and premium.

### English Hero

Eyebrow:

`CNC Machining Taiwan | Prototype to Low-Volume Production`

H1:

`Taiwan CNC Precision Machining Partner`

Subtitle:

`Prototype, low-volume and high-mix precision machining with CMM inspection support for overseas buyers and engineering teams.`

Badges:

- ISO 9001
- CMM Inspection
- Prototype & Low-Volume
- 24/7 Machining Support

CTA buttons:

- Send Drawing
- View Capabilities

### Traditional Chinese Hero

Eyebrow:

`台灣 CNC 精密加工｜打樣到小量量產`

H1:

`台灣 CNC 精密加工協力夥伴`

Subtitle:

`支援打樣、小量與高混低量精密加工，並提供三次元量測支援，協助國內外採購與工程團隊穩定推進專案。`

Badges:

- ISO 9001
- 三次元量測
- 打樣與小量
- 24 小時加工支援

CTA buttons:

- 傳圖評估
- 查看加工能力

Hero visual:

- Use the existing real factory / parts image, but present it inside a premium media card.
- Apply subtle dark overlay.
- Add thin metallic border.
- Add soft shadow.
- Add caption in a glass-style overlay.

Hero caption English:

`Real machining capability, measurable quality and responsive RFQ support.`

Hero caption Chinese:

`真實加工能力、可驗證品質與快速詢價支援。`

Remove the three KPI cards from the Hero. Put them in the next section.

---

## 7. Trust Bar / Why Jintat

Create a clean trust section immediately after Hero.

Section title English:

`Why buyers work with Jintat`

Section title Chinese:

`為什麼客戶選擇瑨達`

Intro English:

`We combine real machining experience, inspection capability and responsive communication to support prototype and low-volume precision parts.`

Intro Chinese:

`我們以真實加工經驗、量測能力與快速溝通，支援打樣、小量與高混低量精密零件需求。`

Cards:

1. English title: `Since 2005`  
   English text: `Long-term machining experience supporting real production needs.`  
   Chinese title: `2005 年起累積經驗`  
   Chinese text: `長期累積加工經驗，支援真實量產與打樣需求。`

2. English title: `CMM + Keyence`  
   English text: `Inspection support for critical dimensions and reports.`  
   Chinese title: `三次元 + Keyence`  
   Chinese text: `支援關鍵尺寸量測與檢驗報告。`

3. English title: `Prototype Friendly`  
   English text: `Trial orders and early-stage engineering samples are welcome.`  
   Chinese title: `歡迎打樣試單`  
   Chinese text: `可從工程樣品、試單與小批量開始合作。`

4. English title: `Responsive RFQ`  
   English text: `Drawing review, DFM feedback and practical manufacturing discussion.`  
   Chinese title: `快速詢價回應`  
   Chinese text: `協助圖面評估、DFM 回饋與製程討論。`

---

## 8. Capabilities Section

Section id: `capabilities`

Title English:

`Machining and process capability`

Title Chinese:

`加工與製程能力`

Intro English:

`From turning and milling to finishing coordination, Jintat supports precision parts that require practical manufacturing review and stable execution.`

Intro Chinese:

`從車削、銑削到表面處理協調，瑨達支援需要製程評估與穩定執行的精密零件。`

Capability cards:

1. CNC Turning / CNC 車削
2. CNC Milling / CNC 銑削
3. C-axis Machining / C 軸加工
4. 4-axis Milling / 四軸銑削
5. Fixture & Jig Parts / 治具與夾具零件
6. Shafts & Sleeves / 軸類與套筒零件
7. Surface Finish Coordination / 表面處理協調
8. Inspection Support / 量測檢驗支援

Each card should be concise.

No long paragraphs.

---

## 9. Industries Section

Section id: `industries`

Title English:

`Industries we support`

Title Chinese:

`應用產業`

Intro English:

`We focus on precision mechanical components where tolerance, delivery, inspection evidence and communication matter.`

Intro Chinese:

`我們聚焦公差、交期、量測證明與工程溝通都很重要的精密機械零件。`

Industry cards:

1. Semiconductor Equipment  
   半導體設備  
   `Fixtures, frames, precision mechanical parts and tooling support.`  
   `治具、框架、精密機構件與設備零件支援。`

2. Industrial Automation  
   工業自動化  
   `Machine components, brackets, shafts, jigs and custom parts.`  
   `機械零件、支架、軸類、治具與客製零件。`

3. Medical Devices  
   醫療器材  
   `Precision stainless, aluminum and engineering material components.`  
   `白鐵、鋁合金與工程材料精密零件。`

4. Aerospace & Defense  
   航太與國防  
   `High-reliability mechanical parts with inspection evidence.`  
   `重視可靠度與量測證明的精密機械零件。`

5. Robotics  
   機器人  
   `Structural parts, motion-related components and prototype iterations.`  
   `結構件、傳動相關零件與打樣迭代支援。`

6. Industrial Machinery  
   產業機械  
   `Turning and milling parts for machinery builders and system integrators.`  
   `支援設備商與系統整合商的車銑加工零件。`

Make cards more premium than current KPI boxes.

Use hover effect:

- subtle translateY(-4px)
- brighter border
- slightly stronger shadow

---

## 10. Proof of Capability Section

Section id: `proof`

Title English:

`Proof of capability`

Title Chinese:

`能力證明`

Subtitle English:

`Real machines, real inspection workflow and real parts help buyers evaluate capability before sending drawings.`

Subtitle Chinese:

`真實機台、真實量測流程與實際零件，協助客戶在寄圖前確認加工能力。`

Use existing gallery images.

Requirements:

- Uniform image ratio, preferably 4:3 or 16:10
- Rounded corners
- Dark overlay captions
- Smooth hover zoom
- Keep lightbox
- Avoid random masonry that looks messy
- Use a clean responsive grid

Captions should be natural, not keyword-stuffed.

Example captions:

English:
- CNC production line
- CMM inspection workflow
- Finished precision components
- Keyence measurement support
- Turned and milled parts

Chinese:
- CNC 生產現場
- 三次元量測流程
- 精密加工成品
- Keyence 量測支援
- 車銑加工零件

---

## 11. Machine & Inspection Equipment Section

Current machine list image `機台清單.jpg` can be kept.

But do not display it like a raw pasted image.

Create a premium equipment section.

Title English:

`Machine list & inspection equipment`

Title Chinese:

`車銑設備與量測設備`

Intro English:

`Our equipment supports turning, milling, C-axis machining, 4-axis milling and inspection for prototype and low-volume production.`

Intro Chinese:

`我們的設備支援車削、銑削、C 軸、四軸加工與打樣小量生產所需的量測檢驗。`

Keep the current equipment table, but make it visually cleaner.

Table columns:

English:
- Category
- Equipment
- Buyer Value

Chinese:
- 類別
- 設備
- 對客戶的價值

Important:

The table currently has only English text. Add Chinese version using `data-i18n` or provide bilingual rows cleanly.

---

## 12. Quality & Documentation Section

Section id: `quality`

Title English:

`Quality that buyers can verify`

Title Chinese:

`讓客戶看得見的品質`

Intro English:

`For precision machining, quality should not rely on words alone. Critical dimensions can be checked with CMM and measurement support according to project requirements.`

Intro Chinese:

`精密加工的品質不應只靠口頭承諾。關鍵尺寸可依專案需求透過三次元與量測設備進行驗證。`

Quality cards:

1. ISO 9001  
   `Quality system management and process control.`  
   `品質系統管理與製程管制。`

2. Mitutoyo CMM  
   `Critical dimension verification and inspection report support.`  
   `關鍵尺寸量測與檢驗報告支援。`

3. Keyence Measurement  
   `Vision measurement support for drawing requirements.`  
   `影像量測支援，貼合圖面要求。`

4. Inspection Reports  
   `Measurement records can be provided according to project needs.`  
   `可依專案需求提供量測紀錄。`

5. Material Certificate  
   `Material documentation can be coordinated when required.`  
   `如專案需要，可協調材質證明文件。`

6. DFM Feedback  
   `Tolerance, material and process risks can be reviewed before production.`  
   `生產前可協助檢視公差、材質與製程風險。`

---

## 13. RFQ / Contact Section

Section id: `contact`

Make this section more powerful and more direct.

Title English:

`Send your drawing for review`

Title Chinese:

`寄圖給我們評估`

Subtitle English:

`Trial orders, prototypes and low-volume RFQs are welcome. Send STEP, DWG or PDF files with material, quantity, tolerance highlights and target delivery date.`

Subtitle Chinese:

`歡迎試單、打樣與小批量詢價。請提供 STEP、DWG 或 PDF 圖檔，並附上材質、數量、關鍵公差與期望交期。`

CTA button English:

`Email RFQ Now`

CTA button Chinese:

`立即寄圖詢價`

Keep mailto link.

Contact info layout:

- Email
- Mobile
- TEL
- RFQ subject suggestion
- RFQ checklist

RFQ checklist:

English:
- Part name
- Material
- Quantity
- Critical tolerance
- Surface finish
- Target delivery date
- Application notes

Chinese:
- 零件名稱
- 材質
- 數量
- 關鍵公差
- 表面處理
- 期望交期
- 用途備註

---

## 14. FAQ Section

Rename current `SEO / AEO Answers`.

Use:

English:
`Buyer Questions`

Chinese:
`採購常見問題`

Intro English:

`Quick answers for buyers before sending drawings.`

Intro Chinese:

`協助採購在寄圖前快速了解合作方式。`

FAQ should not look like SEO text.

It should look like real buyer support.

Keep FAQ structured data in JSON-LD.

Visible FAQ questions may include:

1. What does Jintat Industrial do?  
   瑨達工業主要做什麼？

2. Does Jintat support overseas buyers?  
   瑨達是否支援海外客戶？

3. Can Jintat handle prototype and small-batch CNC machining?  
   瑨達是否能支援打樣與小批量加工？

4. What files should buyers send for RFQ?  
   詢價時應該提供哪些圖檔與資訊？

5. Does Jintat provide inspection reports?  
   瑨達是否能提供量測報告？

6. Which industries does Jintat support?  
   瑨達支援哪些產業？

---

## 15. Footer

Footer should be simple and premium.

Include:

- Jintat Industrial Co., Ltd.
- 瑨達工業有限公司
- CNC Machining Taiwan
- Prototype & Low-Volume
- ISO 9001
- CMM Inspection Reports
- Email
- Phone
- Copyright

Avoid clutter.

---

## 16. Animation and Interaction

Use subtle interactions only.

Allowed:

- Hover lift on cards
- Border glow on hover
- Subtle image zoom
- Smooth menu open/close
- Soft fade-in if simple and not heavy

Avoid:

- excessive moving particles
- spinning logos
- distracting animations
- performance-heavy effects

This is Jintat, a precision machining company, not a gaming website.

---

## 17. Responsive Requirements

Desktop:

- Max content width around 1120px to 1240px
- Hero two columns
- Capabilities grid 4 columns or 3 columns
- Gallery grid 3 columns or 4 columns depending image count

Tablet:

- Hero can remain two columns if space allows
- Cards reduce to 2 columns

Mobile:

- Hero becomes single column
- H1 around 34px
- Buttons full width or easy to tap
- Cards single column
- Gallery single column or 2 columns only if images remain clear
- Contact grid single column
- Hamburger nav active
- No horizontal scroll

Use media queries carefully.

---

## 18. Technical Requirements

The site appears to use a single `index.html` with inline CSS and JS.

You may keep inline CSS if that is simplest.

But organize CSS sections clearly:

```css
/* Variables */
/* Base */
/* Navigation */
/* Hero */
/* Sections */
/* Cards */
/* Gallery */
/* Contact */
/* FAQ */
/* Lightbox */
/* Responsive */
```

Do not introduce heavy frameworks.

Do not require build tools.

This must continue working on GitHub Pages as a static site.

---

## 19. Language Switch Requirements

The existing system uses elements like:

```html
<span data-i18n="en" class="show">English</span>
<span data-i18n="zh">中文</span>
```

Continue using this system.

All new text must have both versions.

For block-level content, follow the existing pattern.

After changes, verify:

- English mode shows only English
- Chinese mode shows only Traditional Chinese
- Language preference persists through localStorage
- No mixed language appears unless intentionally bilingual contact labels are used

---

## 20. SEO Protection

Keep these intact unless improving carefully:

- title
- meta description
- meta keywords
- robots
- author
- canonical
- OG tags
- Twitter tags
- Organization JSON-LD
- WebSite JSON-LD
- FAQPage JSON-LD

You may update visible headings for design, but do not remove SEO content.

If FAQ visible content changes significantly, keep FAQ JSON-LD aligned.

---

## 21. Accessibility

Add or preserve:

- meaningful alt text
- accessible buttons
- aria-label for hamburger menu
- aria-expanded for menu button
- focus states
- sufficient contrast
- keyboard close for lightbox and menu if possible

Do not make text too low contrast.

---

## 22. Final Acceptance Checklist

Before finishing, verify:

- Desktop layout looks premium and clean
- Mobile layout does not break
- No horizontal scrolling
- Hamburger menu works
- Language switch works
- Send Drawing mailto works
- Contact mailto works
- Lightbox works
- Existing images load
- Machine list image still loads
- SEO meta remains
- JSON-LD remains valid enough
- FAQ title is no longer `SEO / AEO Answers`
- Hero is less crowded than before
- Visual design is black / graphite / metallic, not bright blue SaaS template
- All new text has English and Traditional Chinese

---

## 23. Implementation Priority

If time is limited, prioritize in this order:

1. Preserve functionality and SEO
2. Fix overall visual system
3. Redesign Hero
4. Add mobile hamburger nav
5. Improve section order and spacing
6. Improve cards and gallery
7. Polish contact and FAQ
8. Final responsive cleanup

---

## 24. Final Note

Do not simply make the current website darker.

The goal is to rebuild the visual hierarchy so the website feels like an international precision manufacturing brand.

The design should communicate:

- real CNC capability
- real inspection capability
- responsive communication
- trial order friendly
- reliable Taiwan manufacturing partner

End result: a premium, clean, bilingual CNC machining website that overseas buyers can trust.
