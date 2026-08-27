---
name: keyword-driven-internal-linking-optimizer
description: "Use when adding or recommending internal links using primary/secondary keywords and verified site URLs. Prioritize exact keyword URLs, then keyword-containing URLs, then closest relevant URLs."
---
 
# Keyword-Driven Internal Linking Optimizer
 
## Purpose
 
Improve the internal linking of an existing article or webpage by connecting relevant primary and secondary keywords in the content to the strongest verified internal destinations.
 
The skill must:
 
- Use primary and secondary keywords already used in the article as internal-link anchor text.
- Select destinations from verified internal URLs.
- Prioritize URLs according to keyword-to-URL relevance.
- Strengthen topical relationships between pages.
- Help clarify website structure and relationships between broader and narrower topics.
- Avoid irrelevant, forced, repetitive, invented, or guessed links.
- Preserve the article's readability, meaning, and existing URL.
Internal links should help the reader first while also reinforcing clear topical relationships across the website.
 
---
 
# Source Hierarchy
 
Use internal-link information in this order:
 
1. Supplied sitemap URLs
2. Supplied internal-link opportunity data
3. Verified internal URLs supplied by the user
4. Relevant internal pages whose URLs and content are actually accessible
5. Existing internal links already present in the article
Never invent an internal URL.
 
Never assume that a URL exists because its structure appears predictable.
 
Never add a link based only on a guessed URL pattern.
 
## URL Verification Behavior
 
A URL may be described as verified only when it was directly supplied as verified, appears in a supplied sitemap or trusted internal-link dataset, or was actually checked through available website access.
 
When website access is available, verify candidate destination URLs before using them when verification is necessary.
 
When website access is unavailable, rely only on supplied sitemap URLs, supplied verified internal URLs, supplied internal-link data, and existing article links whose destinations are already established in the task context.
 
Do not claim that a URL was checked, accessible, live, or verified unless that status was actually established from the available inputs or tools.
 
---
 
# Core Internal-Linking Principle
 
An internal link is eligible only when the destination is genuinely relevant to:
 
- The keyword used as anchor text
- The surrounding sentence or paragraph
- The reader's likely intent
- The topic of the article
- The destination page's apparent purpose
**Relevance is a mandatory eligibility requirement.**
 
After irrelevant destinations have been removed, apply the URL-selection priority rules below.
 
A keyword match in a URL must never override obvious topical or search-intent mismatch.
 
---
 
# Keyword Identification
 
Before selecting links, identify the article's:
 
- Primary keyword
- Secondary keywords
- Relevant semantic variants when supplied
- Existing keyword phrases that can naturally function as anchor text
Prefer explicitly supplied keyword data.
 
When keyword data is not separately supplied, identify candidate primary and secondary keywords from the article conservatively.
 
Do not invent commercially important keywords that the article does not actually target.
 
---
 
# Anchor Text Rules
 
## Primary Rule
 
Use the **primary and secondary keywords already appearing in the article as anchor text** whenever a relevant internal destination exists.
 
Preferred anchor hierarchy:
 
1. Exact primary keyword
2. Exact secondary keyword
3. Other supplied target keyword already appearing naturally in the article
4. Natural grammatical form of one of those keywords when exact wording would make the sentence awkward
The anchor should normally correspond closely to the topic of the destination page.
 
## Exact Keyword Preference
 
When the article naturally contains:
 
`creatine monohydrate`
 
prefer:
 
`[creatine monohydrate](verified-internal-url)`
 
rather than:
 
`[learn more](verified-internal-url)`
 
or:
 
`[click here](verified-internal-url)`
 
Do not replace good existing prose merely to force an exact-match anchor.
 
If the exact keyword appears several times, link the occurrence that:
 
- Provides the strongest contextual connection
- Appears in a useful explanatory section
- Best helps the reader discover the destination
- Does not interfere with another important link
## Anchor Restrictions
 
Do not:
 
- Use vague anchors such as "click here", "read more", or "this page" when a keyword anchor is available.
- Create unnatural sentences solely to insert a keyword.
- Link every occurrence of a keyword.
- Repeatedly use the same keyword to link to the same URL without a clear reason.
- Use an anchor whose meaning does not accurately describe the destination.
- Modify the factual meaning of the article to accommodate a link.
- Keyword-stuff anchor text.
---
 
# URL Selection Priority
 
For every keyword selected as a possible anchor, identify all **relevant and verified** candidate destinations.
 
Then apply the following hierarchy.
 
## Priority 1 — Exact Keyword URL Match
 
Give the highest priority to a URL whose normalized path or slug directly matches the keyword.
 
Example:
 
Keyword:
 
`creatine monohydrate`
 
Preferred URL:
 
`https://example.com/creatine-monohydrate/`
 
Treat differences in normal URL formatting such as spaces versus hyphens, capitalization, or trailing slashes as equivalent when evaluating the match.
 
An exact URL match should normally win when the page is relevant to the keyword's meaning and intent.
 
---
 
## Priority 2 — URL Contains the Exact Keyword
 
If no appropriate exact-match URL exists, prioritize a verified URL containing the exact keyword phrase within a broader URL path or slug.
 
Example:
 
Keyword:
 
`creatine monohydrate`
 
Candidate:
 
`https://example.com/guides/best-creatine-monohydrate-products/`
 
This ranks below a clean exact-match destination but above a URL that is only semantically related.
 
The destination must still be relevant to the surrounding article context.
 
---
 
## Priority 3 — Closest Relevant URL
 
If no URL satisfies Priority 1 or Priority 2, choose the verified internal URL most closely related to:
 
- The keyword's meaning
- Search intent
- Article context
- Destination page topic
- User journey
- Website hierarchy
Relevant destinations may include:
 
- Product pages
- Service pages
- Category pages
- Collection pages
- Guides
- Ingredient pages
- Educational pages
- Blog posts
- Related taxonomy pages
- Comparison pages
- FAQ resources
- Contact, booking, quote, purchase, or other conversion pages
Choose the destination providing the strongest useful relationship rather than merely the URL with the most overlapping words.
 
---
 
# Candidate Selection Logic
 
Use this process for each primary or secondary keyword.
 
### Step 1: Confirm Anchor Availability
 
Verify that the keyword appears naturally in the article.
 
Prefer an existing occurrence rather than inserting unnecessary new keyword usage.
 
### Step 2: Find Verified Candidate URLs
 
Search only verified internal sources such as:
 
- Supplied sitemap
- Internal-link dataset
- Supplied internal URLs
- Accessible pages from the same website
### Step 3: Remove Ineligible Candidates
 
Reject destinations that are:
 
- Irrelevant
- Only weakly connected to the keyword
- Misaligned with the surrounding context
- On a different website
- Unverified
- Invented
- Based on guessed URL patterns
- The same URL as the current article
### Step 4: Apply URL Priority
 
Among the remaining candidates, rank:
 
1. Exact keyword URL match
2. URL containing the exact keyword
3. Closest semantically relevant URL
### Step 5: Resolve Multiple Candidates
 
When several URLs have the same priority level, prefer the destination with the strongest:
 
1. Search-intent match
2. Topical relevance
3. Contextual fit with the paragraph
4. Relationship to the keyword
5. Reader usefulness
6. Website-hierarchy usefulness
7. Conversion relevance, when appropriate
Do not choose a less relevant page solely because it contains more keyword tokens.
 
---
 
# Internal Linking Placement
 
Insert links where they naturally help the reader.
 
Good placements include:
 
- The first strong contextual mention of a primary or secondary keyword
- A definition of an important concept
- A paragraph introducing a related product or service
- A section discussing a category or subtopic
- A comparison section
- A recommendation or selection section
- A paragraph that naturally leads to a more detailed guide
- A relevant FAQ answer
Avoid placing links:
 
- In headings unless specifically requested
- In every paragraph
- On repeated occurrences of the same keyword
- Where the destination adds no additional value
- Where the link disrupts readability
- Inside quotations
- Inside code
- Inside schema unless the schema specifically requires the URL
- In places where another link already serves the same purpose
---
 
# Link Frequency and Duplication
 
Use a reasonable number of internal links based on:
 
- Article length
- Number of genuinely relevant keywords
- Available verified destinations
- Page purpose
- User journey
Quality takes priority over quantity.
 
Do not repeatedly link to the same destination unless separate links serve clearly different reader needs.
 
Normally, one strong contextual link to a destination is preferable to repeatedly linking the same page.
 
Do not force an internal link for every primary or secondary keyword if no sufficiently relevant destination exists.
 
---
 
# Keyword Cannibalization and Site Structure
 
Use internal links to clarify relationships between related pages.
 
Where appropriate:
 
- Link broader concepts to more specific pages.
- Link specific topics back to useful parent categories or comprehensive guides.
- Distinguish informational pages from commercial pages.
- Help users move logically between products, categories, services, guides, and supporting content.
- Avoid creating misleading signals between pages targeting materially different search intents.
Internal linking should reinforce which destination provides the deeper or more specific treatment of a keyword.
 
Do not solve possible keyword cannibalization by forcing links between unrelated pages.
 
---
 
# CTA Internal Links
 
When CTA data is supplied:
 
- Use the supplied CTA URL.
- Use the supplied CTA anchor text when explicitly required.
- Confirm the destination is internal and verified.
- Keep the CTA visually and contextually distinct from educational links and independent external citations.
When CTA data is not supplied, add a CTA link only when:
 
- It naturally fits the page type
- It supports the business goal
- A verified internal destination exists
- It helps the reader take a logical next step
Do not create or guess a conversion URL.
 
Keyword-anchor requirements do not override explicitly supplied CTA anchor text.
 
---
 
# Relationship to External Citations
 
Do not present an internal business page as independent evidence.
 
Internal links and external citations serve different purposes:
 
**Internal links**
 
- Help navigation
- Connect related website topics
- Support website hierarchy
- Guide users to relevant products, categories, services, or resources
**External citations**
 
- Support factual claims
- Provide independent evidence
- Reference authoritative external sources
Never imply that an internal page independently verifies a factual, scientific, regulatory, medical, legal, or financial claim.
 
---
 
# Existing Links
 
Review existing internal links before adding new ones.
 
Retain an existing link when:
 
- The destination remains relevant
- The anchor is accurate
- The URL is verified
- It provides useful navigation
Improve an existing link when:
 
- A primary or secondary keyword would make a stronger anchor
- A more relevant verified destination exists
- The current anchor is vague
- The current destination no longer represents the strongest topical relationship
Remove an existing internal link when:
 
- It is irrelevant
- It points to an unverified destination
- It duplicates another link without value
- Its anchor misrepresents the destination
Do not change external links unless the user asks for external-link optimization.
 
---
 
# Internal Linking Recommendation Format
 
When the user requests recommendations rather than direct article editing, provide each recommendation with:
 
- **Keyword**
- **URL**
- **Suggested anchor text**
- **Recommended placement**
- **URL priority**
- **Why the destination is relevant**
Use one of these URL-priority labels:
 
- `Priority 1 — Exact keyword URL`
- `Priority 2 — URL contains exact keyword`
- `Priority 3 — Closest relevant URL`
Prioritize the strongest and most useful recommendations.
 
Do not inflate the list with weak opportunities.
 
---
 
# Direct Article Editing Mode
 
When the user asks to add internal links directly to an article:
 
1. Preserve the original article's meaning.
2. Preserve the current page URL.
3. Identify primary and secondary keywords.
4. Find verified relevant destinations.
5. Apply the URL-selection hierarchy.
6. Link natural occurrences of the relevant keywords.
7. Avoid unnecessary rewriting.
8. Return the completed article with the internal links inserted.
Unless requested otherwise, do not clutter the finished article with explanations or SEO notes.
 
---
 
# Recommendation Mode
 
When the user asks for an internal-link audit, opportunities, or recommendations instead of a rewritten article, return the strongest opportunities in descending priority.
 
For each recommendation provide:
 
**Keyword:** [Primary or secondary keyword]
**Suggested anchor text:** [Keyword as it appears in the article]
**Destination URL:** [Verified URL]
**Priority:** [1, 2, or 3]
**Placement:** [Where the anchor occurs or should occur]
**Reason:** [Concise explanation of topical and contextual relevance]
 
---
 
# Tie-Breaking Rules
 
If two destinations appear equally suitable, use the following order:
 
1. Better search-intent alignment
2. More specific topical match
3. Stronger contextual fit
4. Cleaner keyword-to-URL relationship
5. More useful next step for the reader
6. Stronger site-hierarchy relationship
7. More commercially useful destination when commercial intent is appropriate
Do not select a destination purely because it is a product or conversion page.
 
Reader intent and relevance remain mandatory.
 
---
 
# Failure Rules
 
If no suitable verified internal destination exists for a keyword:
 
- Do not invent a URL.
- Do not guess a URL.
- Do not link to an irrelevant page.
- Do not weaken relevance standards merely to create a link.
- Leave the keyword unlinked.
If an exact-match URL exists but its topic or intent does not match the keyword in context:
 
- Reject it.
- Evaluate Priority 2 candidates.
- If necessary, evaluate Priority 3 candidates.
If no appropriate candidate remains, omit the link.
 
---
 
# Final Quality-Control Gate
 
Before returning the result, silently verify:
 
## Keyword Anchors
 
- Anchor text uses primary or secondary keywords from the article wherever appropriate.
- Exact keyword anchors are used naturally.
- No anchor was artificially inserted merely to create a link.
- Anchor text accurately describes the destination.
- No vague anchor is used when a suitable keyword anchor is available.
## Destination Selection
 
- Every destination is internal.
- Every URL is verified.
- No URL was invented.
- No URL was inferred solely from a guessed pattern.
- Every destination is contextually relevant.
- Exact keyword URLs received highest priority among relevant candidates.
- Keyword-containing URLs received second priority.
- Semantically closest URLs were used only when stronger matches were unavailable.
- Search-intent mismatch was not overridden by lexical URL matching.
## Link Quality
 
- Links improve navigation or clarify website structure.
- Link quantity is reasonable.
- Duplicate destination links are avoided unless justified.
- The current page does not link to itself.
- No irrelevant internal links were added.
- Existing useful links were preserved where appropriate.
## Site Structure
 
- Broader and narrower topics are connected logically.
- Links support rather than confuse page intent.
- Internal links do not create unnecessary keyword cannibalization.
- Product, category, informational, and conversion destinations are used according to context.
## CTA
 
- Supplied CTA data is followed exactly when provided.
- CTA destinations are verified.
- CTA links remain distinct from informational links and independent evidence.
## Output
 
- The requested mode was followed.
- No invented URLs appear.
- No hidden reasoning or chain-of-thought is exposed.
- Recommendations contain keyword, anchor, URL, placement, priority, and relevance when requested.
---
 
# RUNTIME INPUTS
 
The current task prompt may contain dynamically populated data from the user's workflow, automation system, API, CMS, files, or other connected data sources.
 
Treat values supplied in the current prompt as the authoritative runtime inputs for this skill. The upstream system may already have resolved template variables before the task reaches the LLM.
 
Do not attempt to resolve, replace, or reconstruct upstream template variables.
 
Possible runtime inputs include:
 
## Article Inputs
 
- Current article URL
- Full article or webpage content
## Keyword Inputs
 
- Primary keyword
- Secondary keywords
- Relevant semantic variants or other supplied target keywords
## Website Inputs
 
- Website domain
- Sitemap or sitemap URLs
- Verified internal URLs
## Internal-Link Inputs
 
- Existing internal links
- Internal-link opportunity data
- Preselected or verified destination URLs
## CTA Inputs
 
- CTA URL
- CTA anchor text
- CTA instructions
## Additional Inputs
 
- Business information
- Page purpose
- Search intent
- Additional task-specific instructions
Not every input will be supplied for every task.
 
Use supplied values when available.
 
For direct article editing, article content is normally required. If the current article URL, keyword data, or CTA data is absent, use the skill's existing fallback rules where applicable rather than inventing missing values.
 
If keyword data is absent, identify candidate primary and secondary keywords from the supplied article conservatively, as defined in this skill.
 
If a sitemap, verified internal URLs, or internal-link opportunity data is absent, use only internal destinations that can actually be verified through available website access.
 
If website access is unavailable, rely only on internal URLs supplied or otherwise verified in the current task context.
 
Never invent missing URLs, sitemap entries, CTA destinations, keywords, business information, or page data.
 
If an unresolved template token appears in the runtime prompt, treat it as unavailable input rather than as meaningful data.
