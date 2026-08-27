---
name: seo-aeo-content-upgrader
description: "Upgrade existing webpages and thin CMS tag pages, or create new research-driven webpages and articles, into accurate, SEO-optimized, AEO-optimized, conversion-focused content. Use this skill when asked to rewrite, expand, restructure, optimize, or create content using page content, sitemap data, keyword data, schema, internal links, search-performance data, business information, audience information, current web research, or additional instructions."
---
 
# SEO and AEO Content Upgrader
 
## Purpose
 
Upgrade existing webpages or create new webpages/articles in the website’s primary language using the supplied page data, sitemap, keywords, schema, links, performance data, business information, audience information, current research, and additional instructions.
 
Produce accurate, useful, search-intent-aligned content that can be implemented in a CMS.
 
Strengthen the content with relevant expert insights, verified statistics, or authoritative citations from non-competitor sources.
 
For new content, research the current topic landscape before selecting or finalizing the angle, terminology, title, keyword strategy, and supporting evidence. Do not rely on stale terminology, outdated assumptions, or historical popularity when the subject has materially changed.
 
This skill supports three operating modes:
 
1. **Standard CMS Page Upgrade**
2. **CMS Tag Page Deep Upgrade**
3. **New SEO/AEO Content Creation**
Follow the mode-selection rules before beginning.
 
---
 
# Mode Selection
 
## Mode A: Standard CMS Page Upgrade
 
Use this mode when:
 
- The user requests optimization of one or more standard webpages.
- Multiple page URLs are supplied.
- The selected page is a product, service, category, article, landing page, informational page, local page, or other non-tag page.
- The user requests CMS-ready content only.
- The user does not explicitly request an SEO analysis package.
Mode A returns only finished, CMS-ready Markdown.
 
Do not include analysis, explanations, strategy notes, keyword reports, editorial comments, implementation notes, or reasoning.
 
## Mode B: CMS Tag Page Deep Upgrade
 
Use this mode when:
 
- The user explicitly asks to improve a tag page.
- The selected page is clearly a CMS taxonomy or tag archive.
- The page has little or no useful original content.
- The user requests keyword extraction, sitemap findings, a content outline, internal-link recommendations, or meta recommendations in addition to the rewritten content.
Mode B returns the complete tag-page analysis and content package defined in the Mode B output contract.
 
## Mode C: New SEO/AEO Content Creation
 
Use this mode when:
 
- The user asks to create, write, generate, draft, or produce a new webpage, article, blog post, guide, comparison, resource, landing-page article, or other content that does not yet have supplied page content to upgrade.
- The user provides a topic, title, content brief, keyword, question set, target audience, business objective, or content-plan item and requests finished new content.
- The user asks the model to research and select a current or trending topic before creating the content.
- The task requires identifying a content gap or a distinct new search intent from the supplied sitemap or website context.
Mode C returns finished, CMS-ready Markdown by default.
 
Research, topic validation, current terminology review, keyword selection, cannibalization checks, source evaluation, and internal-link mapping must happen internally unless the user explicitly requests those materials as separate deliverables.
 
Mode C must not be used to silently replace or rewrite an existing page when full existing page content has been supplied for optimization. Use Mode A or Mode B instead.
 
## Mixed or Ambiguous Requests
 
When several existing pages are supplied, default to Mode A unless the user explicitly requests a separate deep analysis package for every tag page.
 
When a single existing page appears to be a tag page but the user explicitly requests only CMS-ready content, use Mode A and apply the tag-page research process internally.
 
When the request contains both an existing-page upgrade and one or more genuinely new content items, apply the correct mode separately to each deliverable. Do not force new content into Mode A or existing-page rewrites into Mode C.
 
When no existing page content is supplied and the user clearly requests a finished new article or page, use Mode C even if sitemap URLs or other website pages are supplied as references.
 
Never reveal hidden reasoning or chain-of-thought. Provide only the deliverables required by the selected mode.
 
---
 
# Source Hierarchy
 
Use information in this order of authority:
 
1. Supplied business data and explicit user instructions
2. Existing webpage content
3. Product, service, category, and informational pages from the same website
4. Sitemap URLs and URL structures
5. Supplied schema
6. Supplied keyword and performance data
7. Supplied audience, link, image, and conversion data
8. Verifiable contextual information from accessible website pages
9. Original research, public datasets, regulatory guidance, standards, or expert publications from authoritative non-competitor sources
10. General background knowledge that does not create unsupported claims
When two sources conflict, prefer the most direct, specific, current, and authoritative website, business, regulatory, academic, or primary source.
 
Do not treat URL wording alone as proof of a product feature, ingredient, certification, benefit, price, or business claim.
 
If the supplied information is insufficient, write conservatively and omit unsupported details.
 
---
 
# Core Accuracy Rules
 
Do not invent or imply unsupported:
 
- Facts
- Products
- Services
- Ingredients
- Features
- Benefits
- Reviews
- Testimonials
- Ratings
- Statistics
- Prices
- Discounts
- Availability
- Guarantees
- Awards
- Certifications
- Partnerships
- Authors
- Publication dates
- Business credentials
- Scientific findings
- Legal claims
- Medical claims
- Financial claims
- Performance promises
- Expert opinions
- Research findings
- Quotations
- Citations
- Source URLs
Preserve all material facts from the supplied website and business data.
 
When a claim is not directly supported, remove it or rewrite it as neutral educational information.
 
Never fabricate a source, citation, expert, institution, study, quotation, date, statistic, or URL.
 
Do not cite a search-result snippet, AI-generated summary, unsourced content aggregator, or inaccessible reference as though it were the original source.
 
For sports nutrition, supplements, health, wellness, or other regulated topics:
 
- Do not claim that a product diagnoses, prevents, treats, or cures a disease.
- Do not promise guaranteed physical, cognitive, athletic, or health outcomes.
- Do not use “may support,” “designed for,” “commonly used by,” or similar qualifying language unless the underlying statement is supported by the supplied website context or a reliable, directly relevant source.
- Do not transform a weak or unsupported claim into a strong claim.
- Encourage appropriate professional advice only when relevant to the topic and page intent.
- Prefer government agencies, recognized medical institutions, peer-reviewed research, and professional standards bodies.
- Do not rely on commercial supplement brands, competing clinics, competing service providers, or product manufacturers as the primary authority for health claims.
---
 
# URL and Canonical Rules
 
## Modes A and B: Existing Pages
 
The original page URL must never be changed in the completed CMS content.
 
Preserve the original:
 
- Domain
- URL path
- Slug
- Canonical URL
Do not silently create a new URL.
 
In Mode B, the SEO Meta Suggestions section must normally state:
 
**Suggested URL slug: Keep the existing slug.**
 
Only suggest an alternative slug when the user explicitly permits URL changes or requests a migration recommendation. Even then, clearly present it as an optional recommendation and do not replace the original canonical URL in the page content.
 
## Mode C: New Content
 
New content may receive a suggested slug because no existing URL needs to be preserved.
 
The suggested slug must:
 
- Reflect the final topic and primary search intent
- Be concise and readable
- Use natural words rather than keyword stuffing
- Avoid unnecessary dates unless the content is intentionally date-specific
- Avoid inventing a folder structure that cannot be verified from the website
- Follow an existing verified URL pattern only when that pattern is clear from supplied sitemap data
Do not invent or present a live canonical URL for unpublished content.
 
Only include `canonical_url` when the final publishing URL is explicitly supplied or can be deterministically established from user-provided publishing rules. A domain plus a suggested slug is not sufficient evidence to claim that a canonical URL already exists.
 
If the user asks only for CMS-ready new content, provide the suggested slug in front matter and omit `canonical_url` unless it is verified.
 
---
 
# Research and Analysis Process
 
Perform the following work internally before drafting.
 
## 1. Understand the Selected Page
 
Determine:
 
- Page type
- Existing topic
- Business purpose
- Intended audience
- Existing conversion goal
- Primary search intent
- Secondary search intents
- Current content strengths
- Missing information
- Thin, duplicated, outdated, unclear, or unsupported sections
- Whether the page should be improved selectively or rewritten completely
- Which claims would benefit from expert context, research data, or citation support
If existing content is already strong, retain useful material and improve only what is necessary.
 
If it is thin, weak, outdated, duplicated, or missing, create a complete replacement.
 
For Mode C, there may be no selected page to evaluate. Use the new-content process below instead of inventing existing-page observations.
 
## 1A. Define the New-Content Opportunity for Mode C
 
Before drafting new content, determine:
 
- The proposed topic or content brief
- The intended audience
- The business objective
- The desired conversion action, when supplied
- The dominant search intent
- Important secondary intents
- Whether the user supplied a fixed topic or asked the model to discover one
- Whether the subject is fast-moving, moderately evolving, or primarily evergreen
- The primary entity, product, service, problem, question, comparison, or use case the page should own
- Why this content should exist separately from current website pages
- Which existing page is the closest topical neighbor
- Which claims require authoritative evidence
- Which parts of the subject require current verification before writing
Do not begin drafting merely because a keyword or tentative title was supplied. First validate that the proposed angle can support a distinct, useful page.
 
## 1B. Research Freshness, Current Terminology, and Topic Relevance for Mode C
 
When research tools or accessible current sources are available, research the topic before finalizing the title, angle, outline, or keyword set.
 
The purpose of freshness research is to avoid creating content around outdated terminology, obsolete practices, superseded standards, stale statistics, expired trends, or questions that no longer represent the current topic landscape.
 
For fast-moving topics, prioritize current sources and recent developments. Examples include:
 
- Artificial intelligence and software
- Search engines and SEO/AEO/GEO
- Digital marketing platforms
- Laws, regulations, policies, and compliance
- Technology products and standards
- Market conditions
- Current medical or scientific guidance
- Security
- Pricing, availability, product specifications, and platform capabilities
- Current professional practices that change materially over time
For moderately evolving topics, verify that the terminology, recommendations, statistics, and practices remain current before using older material.
 
For stable evergreen subjects, use the most recent authoritative revisions where relevant while retaining older foundational sources when they remain valid.
 
Do not label a topic “trending,” “latest,” “new,” “emerging,” or “current” solely because a recent article exists.
 
A current or trending topic should have evidence such as one or more of the following:
 
- Recent authoritative publications or updates
- A new or materially updated standard, regulation, feature, platform capability, or industry practice
- Multiple recent independent discussions around the same development
- Current search questions or terminology supplied by the user
- Recent public data showing meaningful change
- Current website or performance data showing a relevant content gap or audience need
When the user explicitly asks for a trending or up-to-date topic:
 
- Research before selecting the final topic.
- Prefer developments with clear relevance to the target audience and business.
- Reject outdated angles even when they were historically popular.
- Prefer current terminology used by authoritative sources and the target market.
- Distinguish a temporary news spike from a durable content opportunity.
- Avoid building evergreen content around a fleeting event unless the user explicitly wants news or event coverage.
When the user supplies a fixed topic:
 
- Preserve the requested core subject.
- Research whether terminology, facts, practices, statistics, examples, and supporting questions need updating.
- Modernize outdated terminology only when accuracy and audience usage support the change.
- Retain an older term when it is still necessary for comprehension, standards compliance, historical context, or meaningful search intent.
If current research is unavailable or the user prohibits external research:
 
- Do not claim that the selected topic is trending, latest, or current unless supplied evidence supports that claim.
- Use the supplied data conservatively.
- Avoid time-sensitive facts that cannot be verified.
- Do not invent recent developments to make the content appear current.
## 2. Analyze the Sitemap and Website Context
 
Review the supplied sitemap and accessible internal pages.
 
Identify relevant:
 
- Product pages
- Service pages
- Category pages
- Collection pages
- Blog posts
- Guides
- Ingredient pages
- Educational pages
- Location pages
- Related tags
- Comparison pages
- Frequently asked question pages
- Conversion pages
- Contact, booking, quote, or purchase pages
Look for URLs whose slugs, titles, headings, products, categories, or topics connect meaningfully to the selected page or proposed new content.
 
For Mode C, specifically identify:
 
- Existing pages that already satisfy the proposed intent
- Pages that partially overlap with the proposed topic
- Missing subtopics or unanswered questions
- Natural pillar-and-cluster relationships
- Existing pages that should internally link to the new content when implementation planning is requested
- Existing pages the new content should link to
- Whether the new content would create avoidable keyword or intent cannibalization
Do not create a new page merely because no exact-match URL exists. The content must have a distinct useful purpose.
 
Do not claim that a page was crawled or inspected unless its content was actually supplied or accessible.
 
## 3. Extract Keyword Opportunities
 
Use available information from:
 
- Selected keyword lists
- Ranking keywords
- Search impressions
- Click-through rates
- Search positions
- URL slugs
- Page titles
- Meta titles
- Meta descriptions
- H1, H2, and H3 headings
- Product names
- Service names
- Category names
- Repeated phrases across relevant pages
- Search questions
- Internal anchor text
- Content gaps
- Keyword opportunities supplied by the user
Classify useful terms into:
 
- Primary keyword
- Secondary keywords
- Semantic and related terms
- Long-tail keywords
- Product or category keywords
- Question-based keywords
- URL-derived keywords
- Internal anchor text opportunities
For Mode C, do not rely only on legacy keyword lists or historical terminology when the subject has evolved. Compare supplied terms against current authoritative terminology and current user/search language when research access is available.
 
Do not discard a supplied keyword merely because a newer synonym exists. Determine whether the older term still carries meaningful user intent, and use the most accurate combination of current terminology and relevant search language.
 
## 4. Select the Primary Keyword
 
Choose the best primary keyword based on:
 
- Relevance to the current URL and page purpose
- Search intent
- Existing rankings
- Impressions
- Click-through opportunity
- Ranking position
- Business relevance
- Conversion relevance
- Topical fit
- Keyword cannibalization risk
- Existing keyword use across other supplied pages
Keywords appearing naturally in the selected page URL have priority when they accurately describe the page.
 
Do not force a URL-derived keyword when it conflicts with the page’s actual purpose.
 
For Mode C, where no current page URL exists, select the primary keyword based on the proposed page’s distinct search intent, audience value, business relevance, topical fit, supplied performance data, current terminology, and cannibalization risk. A keyword should not be selected only because it has high volume or appears in a content plan.
 
## 5. Use Performance Data
 
When search-performance data is supplied:
 
- Use high-impression, low-click-through-rate queries to improve the meta title, meta description, introduction, and headings.
- Use relevant queries ranking approximately in positions 4–20 to expand useful content depth.
- Retain relevant terms for which the page already performs strongly.
- Do not replace a successful topic with a less relevant keyword solely because the alternative has higher volume.
- Do not force every supplied keyword into the content.
## 6. Prevent Keyword and Intent Cannibalization
 
When multiple pages are supplied:
 
- Assign each page a distinct primary keyword.
- Assign each page a distinct search intent and content angle.
- Respect the page type, URL, existing content, and business purpose.
- Avoid creating substantially duplicated introductions, headings, FAQ questions, expert insights, or body sections.
- Use internal links to clarify relationships between broader and narrower topics.
- Do not include cross-page cannibalization analysis in Mode A output.
For Mode C:
 
- Compare the proposed article or page against relevant existing sitemap URLs before drafting.
- Do not create a new page that merely rephrases an existing page’s dominant intent.
- Prefer a narrower, broader, comparative, audience-specific, problem-specific, stage-specific, or otherwise distinct angle when that creates genuine user value.
- Do not manufacture artificial differentiation solely to justify another URL.
- When the proposed topic is already well covered, either select a distinct supported gap or follow the user’s fixed topic while avoiding unsupported claims of uniqueness.
- Use internal links to make the relationship between the new page and existing pages explicit.
- Do not expose internal cannibalization analysis in the default Mode C output unless the user requests it.
## 7. Research Expert Insights and Citations
 
Research relevant evidence before drafting the final page.
 
Look for information that can materially improve the reader’s understanding, such as:
 
- Official statistics
- Regulatory guidance
- Industry standards
- Peer-reviewed findings
- Public research
- Professional recommendations
- Definitions from recognized authorities
- Market or consumer data from reputable primary sources
- Technical guidance from standards organizations
- Publicly available expert commentary from qualified individuals or institutions
Prioritize original and authoritative sources, including:
 
1. Government agencies and public institutions
2. Universities and academic institutions
3. Peer-reviewed journals and original research publications
4. Recognized standards bodies
5. Professional associations
6. Established nonprofit research organizations
7. Official public datasets
8. Primary-source statements from qualified experts
9. Independent research organizations with transparent methodology
10. Non-competing technology platforms or industry infrastructure providers when directly relevant
Research must be relevant to the specific page topic and claim.
 
Do not add statistics or expert commentary merely to make the page appear researched.
 
Verify, where available:
 
- Source identity
- Publication or revision date
- Author or issuing organization
- Methodology
- Population or sample
- Geographic relevance
- Whether the source supports the exact claim being made
- Whether newer authoritative evidence supersedes it
Prefer recent sources when the subject changes quickly. For Mode C, actively check whether a newer authoritative source, revision, dataset, standard, regulation, or platform document supersedes an older source before relying on it. Older foundational sources may be used when they remain authoritative and relevant.
 
Use the original source rather than a secondary article whenever the original research, regulation, dataset, or guidance is accessible.
 
## 8. Exclude Competitor Sources
 
Do not use a competitor as the source of an expert insight, statistic, citation, definition, recommendation, or supporting link.
 
Treat a source as a potential competitor when it:
 
- Sells substantially similar products or services
- Targets the same customers with a similar commercial offer
- Operates as a competing agency, consultancy, clinic, platform, retailer, manufacturer, marketplace, publisher, or service provider
- Uses the cited content primarily to promote a competing offer
- Appears in supplied competitor data or is clearly identified by the user as a competitor
Do not cite:
 
- Competitor blog posts
- Competitor service pages
- Competitor product pages
- Competitor case studies
- Competitor surveys created mainly for promotion
- Competitor landing pages
- Affiliate comparison websites
- Commercial listicles promoting competing providers
- Review sites with unclear methodology or commercial conflicts
A source is not automatically a competitor merely because it operates in the same broad industry. Evaluate whether it offers a substantially similar product or service to the same audience.
 
When competitor status is uncertain, prefer a government, academic, regulatory, standards-based, nonprofit, or original public-data source instead.
 
Do not name, quote, link to, or promote a competitor unless the user explicitly requests a competitor comparison.
 
---
 
# Expert Insight and Citation Requirements
 
## Mandatory Placement
 
Insert a relevant expert insight or citation immediately after the first body paragraph of the finished page.
 
The first body paragraph means the first substantive paragraph after the H1. Ignore:
 
- Front matter
- Titles
- Headings
- Breadcrumbs
- Metadata
- Bylines
- Navigation
- Tables of contents
- Disclaimers that appear before the main introduction
The insight placed after the first paragraph must:
 
- Relate directly to the introduction
- Add useful evidence, context, authority, or clarification
- Come from a verified non-competitor source
- Avoid interrupting the natural flow of the page
- Be written for the target audience rather than for search engines
## Additional Placement
 
Add further expert insights or citations only where they improve the content.
 
Appropriate placements may include:
 
- After explaining a key concept
- After introducing an important statistic
- After discussing a common challenge
- After presenting a process or recommendation
- In a section involving health, safety, legal, financial, technical, or regulated information
- After a comparison that benefits from independent context
- Before or after a commercially important decision point
- In a relevant FAQ answer
- Near the conclusion when the evidence supports the next step
Do not add an expert insight or citation to every paragraph.
 
Avoid placing expert insights:
 
- In consecutive paragraphs
- Where they repeat information already established
- Where the source adds no meaningful authority
- Inside a heading
- Inside a quotation
- Inside a code block
- Inside schema
- Between a question and its direct answer
- In a way that disrupts a CTA
For most standard pages, use approximately two to four well-chosen cited insights when the page length and topic support them.
 
Long-form or Mode B pages may contain additional citations, but every citation must remain relevant and useful.
 
## Expert Insight Formats
 
Use one of the following formats based on the page’s tone and CMS conventions.
 
### Integrated Attribution
 
Example:
 
According to the [relevant authority](https://example.org/source), the factor should be evaluated in relation to the user’s specific circumstances rather than in isolation.
 
### Expert Insight Callout
 
Example:
 
> **Expert insight:** The [relevant authority](https://example.org/source) recommends evaluating this factor as part of a broader decision-making process.
 
### Evidence-Based Context
 
Example:
 
Recent data from the [issuing organization](https://example.org/source) indicates that the trend is most relevant when interpreted alongside audience, market, or operational context.
 
Use callout formatting only when it fits the existing page style. Otherwise, integrate the attribution naturally into the paragraph flow.
 
## Citation Style
 
Use descriptive Markdown links.
 
Preferred format:
 
`[Organization or publication name](Exact source URL)`
 
When relevant, identify:
 
- The organization
- The report, standard, study, or guidance
- The publication year
- The expert’s role or qualification
Do not expose raw URLs when descriptive anchor text is more readable.
 
Link directly to the supporting source, report, guidance page, dataset, standard, or research publication whenever possible.
 
Do not link only to a homepage when a more precise source URL is available.
 
Do not add tracking parameters, affiliate parameters, redirects, or shortened URLs.
 
## Quotations and Paraphrasing
 
Prefer accurate paraphrasing over direct quotation.
 
When using a direct quotation:
 
- Verify the exact wording
- Keep the excerpt brief
- Attribute it clearly
- Do not alter the meaning
- Do not imply endorsement of the business, product, or service
- Do not invent quotation marks around a paraphrase
Never write “experts say,” “research proves,” “studies show,” or similar phrases without an identifiable supporting source.
 
Use appropriately cautious wording:
 
- “The source reports”
- “The guidance recommends”
- “The study found”
- “The data indicates”
- “The review concluded”
- “The standard defines”
Do not use “proves” unless the source and claim genuinely justify that wording.
 
## Source Independence
 
Expert insights must remain educational and independent.
 
Do not imply that the cited expert, institution, regulator, university, association, or publication:
 
- Endorses the business
- Recommends the business
- Uses the business’s product
- Has partnered with the business
- Supports the page’s CTA
- Validates a commercial claim beyond the scope of the source
A citation may support a general fact or recommendation without supporting a specific product or service claim.
 
## Citation Failure Rule
 
If no suitable, verifiable, non-competitor source can be found for a proposed claim:
 
- Do not fabricate a citation.
- Do not cite a weak or irrelevant source.
- Remove or soften the unsupported claim.
- Use a different insight that can be supported reliably.
- Omit additional citations rather than lowering source quality.
The mandatory post-introduction insight must still be relevant and supported. Research a broader authoritative context connected to the page topic when a narrowly specific source is unavailable.
 
---
 
# SEO Optimization Requirements
 
Use the selected primary keyword naturally in:
 
- Meta title
- Meta description
- H1
- Introduction
- At least one H2 when appropriate
- Main body content
- FAQ or Q&A content when relevant
- Schema when relevant and factually accurate
Naturally incorporate useful secondary, semantic, related, long-tail, product, category, and question-based keywords.
 
Do not keyword stuff.
 
Prioritize clarity and usefulness over exact-match repetition.
 
Expert insights and citation anchor text must also read naturally. Do not force keywords into source names, quotations, or attribution text.
 
## Meta Title
 
Create a descriptive, click-worthy SEO title.
 
Aim for no more than approximately 60 characters when possible without damaging accuracy or meaning.
 
Do not:
 
- Add unsupported superlatives
- Misrepresent the page
- Use misleading urgency
- Repeat keywords unnaturally
- Insert the business name automatically when it adds no value
## Meta Description
 
Create an accurate, persuasive summary aligned with the page’s search intent.
 
Aim for no more than approximately 155 characters when possible.
 
Include the primary keyword naturally.
 
Do not make claims that the page cannot substantiate.
 
Do not include citation markers or source references in the meta description unless specifically requested.
 
## Headings
 
Use:
 
- One H1 only
- Clear H2 sections
- H3 sections only where they improve organization
- Descriptive headings that communicate the answer or topic
- Natural keyword variations instead of repetitive exact-match headings
Do not create headings solely to contain citations.
 
## Body Content
 
Use:
 
- Short, readable paragraphs
- Clear transitions
- Scannable sections
- Bullet points when useful
- Tables only when they materially improve comparison or comprehension
- Definitions when a term may be unfamiliar
- Practical examples when supported
- Comparisons when meaningful and verifiable
- Direct answers before extended explanations
- Relevant expert insights supported by authoritative non-competitor sources
- Context around statistics so readers understand what the data does and does not show
Avoid:
 
- Filler
- Repetitive summaries
- Generic marketing language
- Empty claims
- Artificial keyword repetition
- Sections that exist only to increase word count
- Citation stuffing
- Decorative statistics with no decision-making value
- Unsupported expert-style language
---
 
# AEO Requirements
 
Structure content so answer engines can identify direct, reliable answers.
 
Where appropriate:
 
- Define the topic early.
- Answer likely questions in the first sentence of a relevant section.
- Use concise answer-first paragraphs.
- Include supporting detail after the direct answer.
- Organize related concepts under descriptive headings.
- Explain who, what, why, when, and how when relevant.
- Include useful comparisons or selection guidance.
- Add an FAQ section only when it contributes meaningful information.
- Keep each FAQ answer accurate, self-contained, and concise.
- Ensure schema exactly matches visible page content.
- Support important factual claims with clear, attributable sources.
- Place the source close to the claim it supports.
- Make the relationship between the claim and source unambiguous.
- Distinguish sourced facts from business-specific statements.
Do not add FAQ content solely to create schema.
 
Do not place citation URLs inside schema unless the selected schema type and property accurately support them.
 
---
 
# Internal Linking Rules
 
Add internal links only when they help the reader or clarify the website structure.
 
Use:
 
- Relevant URLs from the supplied sitemap
- Descriptive, natural anchor text
- Links to closely related product, service, category, guide, ingredient, educational, or conversion pages
- A reasonable number of links based on page length and purpose
When primary and secondary keywords can be used naturally as anchor text for a genuinely relevant internal destination, prefer them or a close natural variation. Do not force an exact-match keyword anchor when it makes the sentence awkward or misrepresents the destination.
 
For Mode C, prioritize internal-link destinations in this order when relevance is otherwise comparable:
 
1. A verified URL whose topic directly matches the anchor concept or exact target keyword
2. A verified URL that clearly contains or targets that keyword concept
3. The closest verified relevant URL that meaningfully helps the reader
Relevance and destination accuracy always override mechanical exact-match linking.
 
Do not:
 
- Link to irrelevant pages
- Repeatedly link to the same destination without a clear reason
- Use vague anchors such as “click here” when a descriptive phrase is available
- Invent URLs
- Add links based only on guessed URL patterns
- Change the current page URL
- Present an internal business page as independent expert evidence
When CTA data is supplied, include one clear CTA using the supplied anchor text and URL.
 
When no CTA data is supplied, create a natural CTA only when appropriate for the page type and business goal. Link it only to a verified internal destination.
 
Keep CTAs visually and contextually distinct from independent citations.
 
Do not imply that an external authority supports the CTA.
 
---
 
# External Linking Rules
 
Include an external link only when it is:
 
- Relevant
- Useful
- Authoritative
- Necessary to support or explain the page topic
- Directly connected to a factual claim, expert insight, definition, standard, dataset, or recommendation
- From a verified non-competitor source
Preferred external sources include:
 
- Government agencies
- Regulators
- Universities
- Peer-reviewed journals
- Standards organizations
- Professional associations
- Established nonprofit organizations
- Official public datasets
- Original research publications
- Qualified experts publishing through reputable institutions
Do not add external links simply to make the page appear researched.
 
Do not send users to competitors unless the user explicitly requests comparisons or external references.
 
Do not use external links from:
 
- Direct commercial competitors
- Competing agencies or consultants
- Competing product or service providers
- Affiliate sites
- Coupon sites
- Low-quality directories
- Content farms
- Scraped publications
- AI-generated source pages
- Unsourced listicles
- Forums or social posts as primary evidence
- Websites with unclear authorship for high-risk claims
A social post may be cited only when the post itself is the subject of the content or when it is an official primary-source statement from a verified institution or qualified expert. Prefer the institution’s official publication when available.
 
Verify that each external URL:
 
- Resolves to the intended source
- Supports the nearby claim
- Does not redirect to a competitor
- Does not contain affiliate or tracking parameters
- Is not a search-results URL
- Is not a fabricated or inferred path
---
 
# Visual and Image Rules
 
When existing image data, image URLs, or image requirements are supplied, include image information only when useful for the CMS page.
 
A useful image recommendation may contain:
 
- Image title
- Suggested filename
- Suggested alt text
- Suggested placement
- Markdown image syntax when a real image URL is supplied
Do not invent image URLs.
 
Do not describe a product image as showing a feature that has not been verified.
 
Write alt text for accessibility and context, not keyword stuffing.
 
Do not add a separate visual-recommendation section unless the selected output mode permits it or the recommendations are directly usable inside the CMS content.
 
Do not use an image caption as a substitute for a proper citation unless the image is the original source of the information.
 
---
 
# Schema Rules
 
Use only schema that accurately represents the final visible page content.
 
Permitted schema types include:
 
- WebPage
- Article
- BlogPosting
- FAQPage
- Product
- Service
- LocalBusiness
- Organization
- BreadcrumbList
- HowTo
Select the most accurate type for the page.
 
Do not create fake or unsupported:
 
- Reviews
- Aggregate ratings
- Prices
- Offers
- Availability
- Authors
- Dates
- Business details
- Locations
- Awards
- Credentials
- Product identifiers
- Citations
- Experts
- Research organizations
If required data is unavailable, omit the unsupported property or omit the schema.
 
Do not output an empty FAQPage object.
 
When FAQ schema is used:
 
- Every schema question must appear visibly in the page.
- Every schema answer must accurately match the visible answer.
- Include only genuine FAQ items.
- Use valid JSON-LD.
Example structure:
 
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "mainEntity": [
    {
      "@type": "Question",
      "name": "Visible FAQ question",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Answer that matches the visible page content."
      }
    }
  ]
}
</script>
 
Do not include schema merely because the original page contains schema. Improve, replace, or omit it based on the final page.
 
---
 
# Mode A: Standard CMS Page Upgrade
 
## Mode A Output Contract
 
Return only the finished, optimized, CMS-ready Markdown.
 
Do not include:
 
- Explanations
- Analysis
- Commentary
- Strategy notes
- Keyword reports
- Keyword maps
- Sitemap findings
- Implementation notes
- Editorial comments
- Content scores
- Checklists
- Introductory or closing remarks
- Separate research notes
- A citation-verification report
- A competitor-source analysis
Research and source evaluation must happen internally.
 
## Single-Page Format
 
Use the following structure when applicable:
 
---
title: "[Optimized page title]"
meta_title: "[Optimized SEO meta title]"
meta_description: "[Optimized SEO meta description]"
slug: "[Existing slug only when supplied]"
tags:
  - "[Relevant tag]"
  - "[Relevant tag]"
categories:
  - "[Relevant category]"
canonical_url: "[Original URL]"
---
 
# [Optimized H1]
 
[Answer-first introduction aligned with the target search intent. Include the primary keyword naturally and make the value of the page immediately clear.]
 
> **Expert insight:** [Relevant evidence, guidance, definition, or context supported by a descriptive link to an authoritative non-competitor source.]
 
## [Descriptive H2]
 
[Useful, accurate body content.]
 
[Add an integrated expert insight or citation here only when it materially supports the section.]
 
## [Descriptive H2]
 
[Useful, accurate body content.]
 
### [Descriptive H3 when useful]
 
[Supporting content.]
 
## [Descriptive H2]
 
[Useful, accurate body content.]
 
## Frequently Asked Questions
 
### [Relevant question]
 
[Clear and accurate answer.]
 
### [Relevant question]
 
[Clear and accurate answer.]
 
## [Relevant CTA heading]
 
[Accurate, contextually appropriate call to action.]
 
[Valid JSON-LD when appropriate.]
 
Include only sections that are useful and supported.
 
The expert-insight callout after the introduction is required, but its wording and format must be adapted to the content. Do not output placeholder text.
 
Additional expert insights should be integrated only where relevant.
 
Do not include:
 
- Empty front-matter fields
- Empty sections
- Placeholder text
- Empty FAQs
- Empty schema
- A CTA when no appropriate conversion action exists
- A tags or categories field when suitable values cannot be inferred safely
- A separate sources section unless the user requests one or the CMS format requires one
- Numbered citations without corresponding visible source details
- Citations to competitors
## Multiple-Page Format
 
For every page, use:
 
<!-- PAGE START: [Original URL] -->
 
[Complete CMS-ready Markdown for this page]
 
<!-- PAGE END: [Original URL] -->
 
Optimize each page separately.
 
Keep every original URL unchanged.
 
Each page must contain its own relevant post-introduction expert insight from a verified non-competitor source.
 
Do not reuse the same insight across pages unless it is independently relevant to each page.
 
Do not place cross-page analysis outside or between page blocks.
 
---
 
# Mode B: CMS Tag Page Deep Upgrade
 
## Tag Page Objective
 
Transform a thin tag or taxonomy page into a complete, useful, commercially relevant, SEO-optimized page that accurately represents:
 
- The tag topic
- Associated products, services, categories, or content
- The user intent behind the tag
- The tag’s relationship to the broader website
- Relevant internal pathways through the website
- Relevant evidence, guidance, or expert context from authoritative non-competitor sources
Target approximately 1,500–2,500 words for the Full Tag Page Content Upgrade unless the user provides a different length.
 
Do not add filler to reach the word target. A shorter, complete, accurate page is preferable to repetitive or speculative content.
 
## Tag Purpose Analysis
 
Determine:
 
- What the tag represents in the website’s context
- Which products, services, articles, categories, ingredients, or topics are associated with it
- Whether the search intent is informational, commercial, educational, transactional, or mixed
- Whether the tag is a product attribute, use case, audience segment, ingredient, goal, category, theme, or editorial topic
- How the tag differs from adjacent categories or tags
- What users should be able to learn, compare, or access from the page
- Which sections would benefit from independent expert evidence or citation support
## Tag Page Content Requirements
 
Create:
 
- One clear H1
- A strong introductory explanation
- A relevant expert insight or citation immediately after the first body paragraph
- Multiple H2 sections
- H3 sections where useful
- Natural internal links
- Relevant comparisons or selection guidance
- Verifiable benefits, use cases, or considerations
- An explanation of who the topic may be relevant for
- A connection to the broader website catalog
- Additional expert insights where they materially strengthen important sections
- FAQs when useful
- A relevant CTA when supported
- Accurate schema when appropriate
Potential H2 coverage includes:
 
- What the tag or topic means on this website
- Related products, services, or categories
- How to understand or compare related options
- Supported benefits, use cases, or considerations
- Who may find the topic relevant
- How the topic connects to the wider catalog
- Related educational resources
- Frequently asked questions
Do not force every topic into every page.
 
Do not force a citation into every section.
 
## Mode B Output Contract
 
Return the following seven sections in this order.
 
### 1. Tag Purpose Summary
 
Briefly explain:
 
- What the tag should represent
- The dominant user intent
- The appropriate content direction
- How the page connects to the website’s products, services, categories, or editorial content
- The type of independent expert evidence most relevant to the page
Keep this section concise.
 
Do not reveal hidden reasoning.
 
### 2. Relevant Sitemap Pages Found
 
List the most relevant verified URLs.
 
For each URL, include:
 
- URL
- Page type
- Why it is relevant to the tag
- How it may support the tag page
Do not list irrelevant URLs to increase the number of findings.
 
Do not invent titles or page details that were not supplied or accessible.
 
Do not present internal website pages as independent expert sources.
 
### 3. Keyword Set
 
Provide grouped keyword recommendations:
 
- Primary keyword
- Secondary keywords
- Long-tail keywords
- Product or category keywords
- URL-derived keywords
- Internal anchor text keywords
Use only keywords that fit the page’s actual topic and intent.
 
Distinguish keyword opportunities from verified search-performance terms when necessary.
 
Do not convert source names or expert terminology into forced keyword targets.
 
### 4. Recommended Page Structure
 
Provide the proposed:
 
- H1
- Introductory paragraph
- Mandatory expert insight or citation after the first paragraph
- H2 headings
- H3 headings where useful
- Additional expert-insight placements where relevant
- FAQ topics where useful
- CTA placement where relevant
The outline must match the full content that follows.
 
For each proposed expert-insight placement, identify the type of evidence to use, such as:
 
- Government statistic
- Regulatory guidance
- Peer-reviewed finding
- Standards definition
- Professional-association recommendation
- Public dataset
Do not recommend competitor sources.
 
### 5. Full Tag Page Content Upgrade
 
Write the complete tag-page content in clean Markdown.
 
Use:
 
- One H1
- Clear H2 and H3 headings
- Short paragraphs
- Useful bullets or tables where appropriate
- Natural internal links
- A helpful, authoritative, brand-appropriate tone
- Commercially useful language without excessive promotion
- A relevant, researched expert insight or citation immediately after the first body paragraph
- Additional non-competitor citations where they materially improve the content
- Accurate FAQs where useful
- A relevant CTA where appropriate
- Valid JSON-LD after the visible content when supported
Do not include analysis notes inside the page content.
 
Do not refer to “the sitemap,” “keyword data,” “SEO analysis,” “the prompt,” “the supplied data,” “competitor screening,” or “the research process” in the customer-facing copy.
 
Do not include a citation in every paragraph.
 
Do not cite competitors.
 
### 6. Internal Linking Recommendations
 
For each recommended internal link, provide:
 
- URL
- Suggested anchor text
- Recommended placement
- Why the destination is relevant
Prioritize the strongest and most useful internal links.
 
Avoid duplicate or forced recommendations.
 
Keep internal linking recommendations separate from independent external citations.
 
### 7. SEO Meta Suggestions
 
Provide:
 
- SEO title, ideally no more than 60 characters
- Meta description, ideally no more than 155 characters
- Suggested URL slug
Unless URL changes were explicitly authorized, write:
 
**Suggested URL slug: Keep the existing slug.**
 
---
 
# Mode C: New SEO/AEO Content Creation
 
## Mode C Objective
 
Create a complete new webpage or article that fills a defensible content need, satisfies a distinct user/search intent, uses current terminology and verified information, supports the website’s topical architecture, and is ready for CMS implementation.
 
Mode C is not a generic article generator. It must use the available website, sitemap, keyword, audience, performance, business, source, and research context to determine what the new page should say and how it should differ from existing content.
 
## Mode C Topic Selection Rules
 
### When the User Supplies a Fixed Topic or Title
 
Keep the core subject unless the user explicitly allows topic replacement.
 
Before drafting:
 
- Verify current terminology and material facts.
- Determine the dominant search intent.
- Identify the closest existing website pages.
- Check for keyword and intent overlap.
- Refine the angle so the page adds distinct value without changing the requested subject.
- Identify current authoritative evidence and relevant questions.
- Avoid obsolete framing even when it appears in older source material.
Do not silently replace the user’s requested topic with a different topic simply because another topic appears more current.
 
### When the User Asks the Model to Select or Propose the Topic
 
Research before choosing the final topic.
 
Evaluate candidate topics using:
 
- Current relevance to the target audience
- Business relevance
- Search-intent clarity
- Topical-authority value
- Evidence of current interest or change when freshness is important
- Available keyword and performance evidence
- Sitemap/content-gap evidence
- Cannibalization risk
- Ability to support the topic with authoritative non-competitor sources
- Durability of the opportunity beyond a short-lived news spike
Reject candidate topics that are:
 
- Already substantially covered by an existing website page
- Based mainly on obsolete terminology or outdated practices
- Supported only by weak, promotional, or competitor sources
- Too broad to satisfy a coherent search intent
- Too narrow to provide meaningful standalone value
- Unrelated to the business, audience, or topical architecture
- Presented as trending without evidence of current relevance
When several candidates are viable, prefer the topic with the strongest combination of distinct user value, current relevance, business fit, authoritative evidence, and internal-link potential.
 
## Mode C Content Planning Requirements
 
Before drafting, internally define:
 
- Primary keyword
- Secondary keywords
- Semantic and related terms
- Search intent
- Article/page angle
- Audience
- Content objective
- Conversion objective, when supplied
- H1
- H2/H3 structure
- Questions worth answering
- Required expert evidence
- Internal-link destinations
- Appropriate CTA, when supported
- Appropriate schema type
- Suggested slug
The structure must follow the subject rather than a fixed template.
 
Do not add sections merely because they are common in SEO articles.
 
## Mode C Content Requirements
 
The finished content should, where appropriate:
 
- Use one clear H1.
- Answer the core intent early.
- Use the primary keyword naturally in the H1, introduction, metadata, and body.
- Use current terminology accurately.
- Explain important concepts before assuming specialist knowledge.
- Include useful H2 and H3 sections based on real sub-intents.
- Use comparisons, steps, examples, definitions, tables, or bullets only when they improve comprehension.
- Include a relevant authoritative expert insight or citation immediately after the first substantive body paragraph.
- Add further citations only where they materially strengthen factual or decision-relevant claims.
- Use verified internal links from the supplied sitemap when useful.
- Use primary or secondary keyword anchors naturally when they accurately describe the destination.
- Include FAQs only when they address genuine questions not already answered adequately in the main body.
- Include a CTA only when a verified destination and appropriate commercial next step exist.
- Add valid JSON-LD only when the schema accurately matches visible content.
Do not copy the structure, phrasing, examples, or distinctive expression of external articles. Research should inform the new content, not reproduce other publishers’ work.
 
## Mode C Freshness and Date Handling
 
For time-sensitive content:
 
- Verify the factual cutoff before writing.
- Use concrete dates when relative wording could become misleading.
- Avoid “currently,” “today,” “latest,” “new,” or similar language unless the claim was verified as current during research.
- Update or omit statistics that have been superseded.
- Prefer the newest authoritative version of rules, standards, specifications, platform documentation, and regulatory guidance.
- Include a year in the title only when the year materially helps the user or the content is intentionally maintained as a date-specific resource.
Do not insert a current year merely as an SEO tactic.
 
For evergreen content, avoid unnecessary date references that will make accurate content appear stale prematurely.
 
## Mode C Output Contract
 
Return only the finished, optimized, CMS-ready Markdown unless the user explicitly asks for a research report, content brief, keyword analysis, source list, or other supporting deliverable.
 
Do not include by default:
 
- Research notes
- Topic-selection analysis
- Competitor-source analysis
- Keyword reports
- Cannibalization reports
- Sitemap findings
- Editorial comments
- Implementation notes
- Content scores
- Checklists
- Hidden reasoning
- Explanations before or after the content
Use the following structure when applicable:
 
---
title: "[Optimized content title]"
meta_title: "[Optimized SEO meta title]"
meta_description: "[Optimized SEO meta description]"
slug: "[Suggested new slug]"
tags:
  - "[Relevant tag]"
categories:
  - "[Relevant category]"
---
 
# [Optimized H1]
 
[Answer-first introduction aligned with the primary search intent and written using current, accurate terminology.]
 
> **Expert insight:** [Relevant evidence, guidance, definition, statistic, or context supported by a descriptive link to an authoritative non-competitor source.]
 
## [Descriptive H2]
 
[Useful, original, accurate body content.]
 
## [Descriptive H2]
 
[Useful, original, accurate body content with internal links where relevant.]
 
### [Descriptive H3 when useful]
 
[Supporting detail.]
 
## Frequently Asked Questions
 
### [Relevant question]
 
[Direct, self-contained answer.]
 
## [Relevant CTA heading]
 
[Accurate, contextually appropriate CTA using a verified internal destination.]
 
[Valid JSON-LD when appropriate.]
 
Include only fields and sections that are useful and supported.
 
For new content:
 
- `slug` is a recommendation for publication, not proof of an existing URL.
- Omit `canonical_url` unless the final publishing URL is explicitly supplied or deterministically verified.
- Omit empty tags, categories, FAQs, CTA sections, and schema.
- Do not output placeholder text.
- Do not invent author names, publication dates, modified dates, or business credentials.
- Do not add a separate sources section unless requested or required by the CMS.
- Do not cite competitors.
- Do not describe the content as “trending,” “latest,” or “up to date” unless the supporting research justifies that description.
---
 
# Language and Brand Voice
 
Write in the website’s primary language.
 
Preserve the language used by the business unless the user explicitly requests translation.
 
Match the supplied brand tone where identifiable.
 
Otherwise use a tone that is:
 
- Helpful
- Authoritative
- Clear
- Accurate
- Accessible
- Commercially useful
- Not excessively promotional
- Evidence-aware without sounding academic unless the audience requires it
Avoid switching languages inside the same page unless necessary for proper names or established terminology.
 
Translate explanatory text when required, but preserve the official names of organizations, reports, standards, journals, and experts when translation would reduce accuracy.
 
---
 
# Final Quality-Control Gate
 
Before returning the output, silently verify all of the following.
 
## Accuracy
 
- Every material claim is supported.
- No product, service, ingredient, feature, or credential was invented.
- Regulated-topic language is appropriately cautious.
- The page does not contradict supplied business data.
- No statistic, quotation, expert, study, institution, or source was invented.
- Every citation supports the exact nearby claim.
- Paraphrases preserve the source’s original meaning.
- Direct quotations are exact and clearly attributed.
## Expert Insights and Citations
 
- A relevant expert insight or citation appears immediately after the first body paragraph.
- Additional insights appear only where useful.
- Citations are not inserted into every paragraph.
- Sources are authoritative and relevant.
- Sources are not competitors.
- No competitor is named, linked to, quoted, or promoted.
- Original sources are used where accessible.
- Time-sensitive information is reasonably current.
- Older sources are used only when still authoritative.
- The source URL is exact and functional.
- Citation anchor text clearly identifies the source.
- No search-result, affiliate, tracking, shortened, or fabricated URL is used.
- No citation falsely implies endorsement of the business.
- No external authority is presented as supporting a CTA.
- Research findings are not overstated.
## URL Integrity
 
- In Modes A and B, the original URL is unchanged.
- In Modes A and B, the canonical URL matches the original URL when supplied.
- In Mode C, the suggested slug is clearly a recommendation for new content.
- In Mode C, no live canonical URL was invented.
- No invented internal URLs appear.
- No unsupported slug replacement was made.
## Search Optimization
 
- The primary keyword matches the page purpose.
- The primary keyword appears naturally in key page elements.
- Secondary and semantic terms are used naturally.
- Search intent is satisfied.
- Content does not compete unnecessarily with other supplied pages.
- Mode C content fills a distinct useful intent or gap rather than duplicating an existing page.
- For Mode C, current terminology was checked when research access and topic volatility made that necessary.
- No keyword stuffing is present.
- Citation text is not manipulated for keyword density.
## Content Quality
 
- There is one H1 only.
- H2 and H3 hierarchy is logical.
- Paragraphs are readable.
- Sections are useful and non-repetitive.
- Direct answers appear early.
- The introduction clearly explains the page value.
- The first expert insight flows naturally from the introduction.
- Additional expert insights add substance rather than decoration.
- Mode C does not use stale facts, obsolete practices, or unsupported “current/trending/latest” framing.
- Mode C terminology reflects current authoritative usage when the subject has evolved.
- The CTA is relevant when included.
- The CTA remains separate from independent evidence.
## Links and Schema
 
- Internal links are relevant and verified.
- Anchor text is descriptive.
- External citations are authoritative, useful, and non-competitive.
- Schema matches visible content.
- JSON-LD is valid.
- No empty or unsupported schema properties appear.
- Citations are not added to schema unless supported by the schema type and visible content.
## Output Compliance
 
- The correct mode was selected.
- Mode A contains only CMS-ready Markdown.
- Mode B contains all seven required sections.
- Mode C contains only CMS-ready Markdown by default unless the user requested supporting analysis.
- Mode C does not invent an existing URL, canonical URL, author, or publication date.
- Mode C performed freshness research when the user requested a current or trending topic and research access was available.
- No unresolved upstream template token is copied into the finished customer-facing content.
- No hidden reasoning or chain-of-thought is revealed.
---
 
# RUNTIME INPUTS
 
The current task prompt may contain dynamically populated values supplied by the user’s upstream workflow, prompt-template system, automation, API, CMS, files, or connected data sources.
 
Treat the resolved values present in the current task prompt as the authoritative runtime inputs for this skill, subject to the Source Hierarchy and explicit user instructions.
 
The upstream system may use template variables before the request reaches the model. This skill does not perform that substitution step.
 
Therefore:
 
- Do not expect skill-local template variables to be populated.
- Do not attempt to resolve, replace, reconstruct, or infer upstream template tokens.
- Use the actual resolved values supplied in the current task prompt.
- Do not require exact field labels when the meaning of the supplied data is clear.
- Not every runtime input will be available for every task.
- Do not require missing optional inputs.
- If a literal unresolved template token is received instead of a usable value, treat that input as unavailable and do not invent the missing value.
- Never copy unresolved template tokens into customer-facing output.
## Page Selection and Existing Content
 
These inputs primarily support Modes A and B:
 
- Selected page URL or URLs
- Selected page full content
- Existing page schema types
- Existing page metadata when supplied
Modes A and B should use these existing-page inputs when they are available.
 
Mode C does not require an existing page URL, existing page content, or existing schema. Do not invent existing-page data for new content.
 
## New-Content Brief
 
These inputs primarily support Mode C:
 
- Topic
- Proposed title
- Content-plan item
- New-content brief
- User questions to answer
- Requested content type
- Search intent or business objective
- Topic-discovery or trending-topic instruction
When the user requests new content, treat the supplied topic, title, brief, content-plan item, or topic-discovery instruction as the governing new-content brief unless explicit instructions state otherwise.
 
## Website and Business Context
 
Possible inputs include:
 
- Website domain or domains
- Website primary language
- Website business name or names
- Business data
- Product or service information
- Brand positioning
- Geographic or market context
Use supplied business information as authoritative for business-specific claims unless stronger explicit instructions or more direct first-party data supersede it.
 
## Sitemap and Website Structure
 
Possible inputs include:
 
- Primary sitemap or sitemap index
- Known website URLs
- Category or taxonomy structure
- Existing content inventory
Use these inputs for topical mapping, cannibalization checks, URL-pattern validation, and internal-link discovery when relevant.
 
## Keyword and Search-Performance Data
 
Possible inputs include:
 
- Primary keyword candidate
- Selected keyword list
- Keywords appearing in an existing page URL
- Search-performance data
- Search Console or other supplied performance metrics
Use supplied keyword and performance data as evidence, not as a requirement to force keywords unnaturally into the content.
 
## Internal-Link Data
 
Possible inputs include:
 
- Preselected internal-link opportunities
- Verified internal URLs
- Preferred anchor targets
- Existing internal-link relationships
Use supplied internal-link data when relevant, while still applying the internal-link quality and verification rules in this skill.
 
## Audience, Conversion, and Media Data
 
Possible inputs include:
 
- Audience data
- Persona or user-intent data
- CTA data
- Conversion objective
- Image or media data
Use these inputs to determine depth, terminology, examples, CTA relevance, and media recommendations where applicable.
 
## Additional Instructions and External References
 
The current task prompt may also contain:
 
- Additional instructions
- Required output constraints
- Reference files
- Public URLs
- GitHub repositories or skill/reference links
- Required external methodologies or frameworks
Apply these according to the Source Hierarchy and the explicit instruction priority defined by the task.
 
When an external reference must be reviewed, do not claim to have applied it unless it was actually accessible and reviewed. If it cannot be accessed, state that limitation when material to the requested deliverable.
 
## Runtime Input Handling by Mode
 
### Mode A
 
Use the supplied existing-page content and page context as the primary working material. Supplement it with supplied website, sitemap, keyword, audience, business, performance, link, and research inputs as applicable.
 
### Mode B
 
Use the supplied tag/taxonomy page context plus sitemap, keyword, internal-link, business, audience, and research inputs to produce the Mode B package.
 
### Mode C
 
Use the supplied new-content brief together with available website, sitemap, keyword, performance, audience, business, CTA, internal-link, media, and research inputs.
 
Existing-page content is optional in Mode C and should only be treated as reference material when the task clearly identifies it as such. Do not convert reference content into an existing-page upgrade unless the user requested that outcome.
