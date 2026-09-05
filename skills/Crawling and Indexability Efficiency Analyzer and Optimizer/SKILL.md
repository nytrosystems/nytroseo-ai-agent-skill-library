⸻name: crawling-indexability-efficiency-analyzer-optimizer 
description: > 
Analyzes and optimizes website discovery, crawling efficiency, rendering, 
technical indexability, canonicalization, XML sitemaps, robots controls, 
internal linking, crawl waste, and search-engine index selection. Use when 
investigating Search Console indexing data, crawl exports, server logs, 
robots.txt, sitemaps, canonicals, noindex directives, redirects, status 
codes, JavaScript rendering, faceted navigation, duplicate URLs, orphan 
pages, crawl traps, migrations, or unexplained indexing problems. Do not use 
for general keyword research or content planning without a crawling or 
indexability question.


Crawling and Indexability Efficiency Analyzer and Optimizer

Purpose

Analyze how efficiently search engines can:

1. discover URLs;
2. crawl URLs;
3. render content where necessary;
4. determine whether URLs are indexable;
5. select canonical URLs;
6. evaluate page quality and uniqueness;
7. include appropriate URLs in their indexes;
8. revisit important URLs efficiently.

Identify technical or structural patterns that waste crawler resources, prevent 
important pages from being discovered or indexed, create conflicting indexing 
signals, or cause low-value URLs to compete with important content for crawler 
attention.

Also identify technical accessibility issues that may reduce the likelihood 
that search engines, AI-powered search systems, answer engines, or other 
retrieval systems can reliably discover and understand useful site content.

The goal is not to maximize the number of indexed URLs.

The goal is to make sure:

- valuable URLs are easy to discover;
- important URLs can be crawled reliably;
- indexable URLs provide sufficient unique value;
- duplicate and low-value URLs are controlled appropriately;
- canonical signals are coherent;
- sitemaps contain the URLs search engines should consider;
- internal architecture communicates importance clearly;
- crawler resources are not consumed unnecessarily;
- search engines receive consistent technical signals.

Core Diagnostic Model

Never treat "indexing" as a single binary state.

For each important URL or URL class, distinguish the following stages.

1. Discoverable

Can a crawler find the URL through mechanisms such as:

- internal links;
- XML sitemaps;
- external links;
- feeds;
- redirects;
- hreflang;
- previously known URLs;
- submitted URLs;
- other discoverable references?

A URL can be indexable but poorly discoverable.

2. Crawlable

Can the crawler request the URL?

Consider:

- robots.txt;
- authentication;
- network accessibility;
- DNS;
- connection failures;
- server availability;
- crawl-rate constraints;
- blocked resources;
- bot protection;
- firewalls;
- CDN behavior.

A URL can be discoverable but not crawlable.

3. Renderable

If important content or links depend on rendering, can the crawler obtain the 
meaningful rendered content?

Consider:

- JavaScript execution;
- client-side rendering;
- server-side rendering;
- hydration;
- API failures;
- blocked resources;
- lazy loading;
- route handling;
- content inserted only after user interaction.

A URL can be crawlable but its meaningful content may not be reliably 
renderable.

4. Indexable

Does the URL permit indexing from a technical-directive perspective?

Consider:

- meta robots;
- X-Robots-Tag;
- HTTP status;
- canonical signals;
- authentication;
- inaccessible content.

A URL can be technically indexable without being selected for indexing.

5. Canonical Candidate

Does the URL appear to search engines to be the preferred representative of its 
content?

Consider:

- rel=canonical;
- redirects;
- internal links;
- sitemap inclusion;
- duplicate content;
- protocol/hostname consistency;
- parameter variants;
- language versions.

Canonicalization signals may conflict.

6. Index-Worthy

Does the page appear sufficiently useful, distinct, stable, and meaningful to 
justify inclusion in a search index?

Consider:

- uniqueness;
- substantive content;
- duplication;
- soft-404 characteristics;
- templated similarity;
- doorway-like patterns;
- empty pages;
- near-empty archives;
- low-value faceted combinations;
- generated pages with no distinct purpose.

Technical indexability does not guarantee index selection.

7. Indexed

Is the URL actually represented in the search engine's index according to the 
available evidence?

Do not infer actual indexing solely because a URL is technically indexable.

Context Handling

Use the invoking prompt as the primary task context.

Read all user-supplied information before beginning analysis.

Relevant inputs may include:

- domain names;
- website URLs;
- page URLs;
- robots.txt;
- XML sitemaps;
- sitemap indexes;
- crawl exports;
- site-audit exports;
- Google Search Console exports;
- indexing reports;
- URL Inspection results;
- screenshots;
- server logs;
- CDN logs;
- status-code reports;
- redirect reports;
- canonical data;
- noindex data;
- internal-link graphs;
- crawl-depth reports;
- orphan-page reports;
- URL parameter reports;
- page templates;
- source code;
- repositories;
- JavaScript applications;
- rendered HTML;
- raw HTML;
- CMS information;
- pagination patterns;
- faceted-navigation patterns;
- hreflang data;
- analytics or traffic data;
- page inventories;
- historic crawl data.

Do not require predefined input fields.

Do not output meaningless template variables.

Do not ask users to restructure data that can already be interpreted from the 
supplied context.

Prompt Precedence

Specific instructions in the invoking prompt take precedence over this default 
workflow.

Examples:

If only robots.txt is supplied, focus on robots behavior.

If the user provides a GSC indexing export, diagnose indexing classifications 
and patterns.

If server logs are provided, perform actual crawler-behavior analysis.

If a crawl export is provided, analyze crawlability and technical signals.

If source code or a repository is supplied, inspect the implementation causing 
crawl or indexing behavior.

If the task concerns one URL, do not force a sitewide audit.

If the user requests only recommendations, keep supporting analysis concise.

Missing Information

Do not guess missing crawler or indexing data.

Never invent:

- crawl frequency;
- crawler request volume;
- server response time;
- crawl budget;
- Googlebot behavior;
- index counts;
- search-console classifications;
- canonical selections;
- log activity;
- traffic;
- rankings;
- crawl demand;
- crawl-rate limits.

When exact data is unavailable:

- use qualitative reasoning;
- identify what can and cannot be established;
- label assumptions;
- distinguish possible causes from confirmed causes.

Do not diagnose "crawl budget" merely because some pages are not indexed.

Data Coverage and Limitations

Before making material diagnoses, state which evidence is available and its 
coverage. Include, where relevant:

- datasets and reports received;
- reporting and log date ranges;
- whether URL data is exhaustive, filtered, or sampled;
- crawl user agent, crawl scope, rendering mode, and crawl configuration;
- Search Console property type, report scope, and known export limitations;
- server-log time zone, filters, exclusions, and crawler-verification method;
- sitemap versions or retrieval times;
- known blind spots or unavailable evidence.

Do not imply sitewide coverage when the evidence represents only a sample or 
limited date range.

Evidence Classification

Classify every material conclusion using one of these evidence states:

Observed 
Directly supported by supplied or researched data.

Correlated 
Supported by multiple datasets showing the same pattern.

Inferred 
Reasonably suggested by available evidence but not directly proven.

Possible Cause 
Plausible but requires verification.

Needs Verification 
Cannot be established from the available evidence.

Also assign a confidence level of High, Medium, or Low and briefly explain the 
basis when confidence is not High.

Treat judgments about content quality, uniqueness, helpfulness, demand, or 
index-worthiness as inferred unless direct evidence establishes the claim.

Do not present a possible cause, inference, or assumption as a confirmed 
diagnosis.

Research Strategy

When external research capabilities are available, conduct relevant research 
before making implementation-sensitive recommendations.

GitHub-First Technical Research

Prioritize GitHub for research involving practical implementation patterns, 
crawler tooling, robots parsers, sitemap generators, crawl libraries, 
framework behavior, CMS implementations, and recurring technical bugs.

Research relevant:

- repositories;
- README files;
- source code;
- issues;
- discussions;
- pull requests;
- tests;
- release notes;
- crawler implementations;
- robots.txt parsers;
- XML sitemap libraries;
- canonical-generation utilities;
- SEO framework components;
- JavaScript rendering tools;
- static-site generators;
- ecommerce platforms;
- CMS plugins;
- log-analysis projects;
- URL-normalization libraries.

Use GitHub especially when diagnosing:

- malformed sitemaps;
- canonical-generation bugs;
- duplicate route generation;
- framework routing;
- JavaScript links;
- client-side rendering;
- pagination;
- faceted URLs;
- CMS plugin conflicts;
- robots generation;
- SSR/CSR differences;
- parameter handling;
- trailing-slash behavior;
- redirect middleware.

GitHub evidence is valuable for understanding real implementation behavior.

Do not treat GitHub projects as the final authority for search-engine crawler 
requirements.

Authoritative Validation

For normative claims about search-engine behavior, crawler directives, 
indexing eligibility, supported controls, or search-engine-specific rules, 
prefer current primary documentation when available.

Examples include:

- official search-engine documentation;
- official robots.txt specifications or standards;
- Schema and web standards where relevant;
- official CMS/framework documentation;
- official HTTP specifications.

If repository behavior conflicts with authoritative documentation, identify the 
implementation as potentially incorrect or outdated.

Research Stopping Rule

Stop external research when all of the following are true:

- relevant protocol or search-engine behavior has been validated;
- the affected URL pattern and likely scope are established;
- the probable root-cause layer is identified or remaining uncertainty is 
- clearly stated;
- an actionable recommendation and verification method can be provided; and
- additional sources are no longer changing the diagnosis or priority.

Do not continue collecting sources merely to make the report appear more 
comprehensive.

Analysis Workflow

1. Establish Site and URL Architecture

Determine the major URL classes.

Examples:

- homepage;
- category pages;
- subcategory pages;
- product pages;
- service pages;
- location pages;
- articles;
- author archives;
- tags;
- search pages;
- pagination;
- filtered URLs;
- faceted combinations;
- tracking parameters;
- session URLs;
- sort URLs;
- internal search;
- media URLs;
- APIs;
- translated URLs;
- utility pages;
- account pages.

Do not analyze thousands of URLs only as individual rows.

Identify template-level and URL-pattern-level behavior.

Sampling Large URL Inventories

When exhaustive analysis is impractical:

- stratify URLs by template, directory, indexability state, status code, 
- traffic or business importance, and other relevant URL classes;
- test representative URLs from each material class;
- state the sample size and selection method;
- distinguish sample observations from sitewide findings;
- avoid extrapolating beyond the evidence without labeling the conclusion as 
- inferred; and
- recommend an expanded or exhaustive test when the sample cannot establish 
- impact or scope reliably.

2. Build a Crawl/Index State Matrix

Where data permits, classify each important URL or URL pattern using dimensions 
such as:
URL / Pattern	Discoverable	Crawlable	Renderable	HTTP Status	Index Directive	Canonical	Sitemap	Internal Links	Search Index State	Evidence Status	Confidence


Use this matrix to identify contradictions.

Examples:

- indexable URL blocked by robots;
- noindex URL included in sitemap;
- redirected URL in sitemap;
- canonicalized URL heavily internally linked;
- 404 URL still linked internally;
- orphan URL included only in sitemap;
- canonical target not internally linked;
- important URL omitted from all discovery mechanisms.

3. Analyze Search Console Indexing Data

When search-engine indexing reports are provided, interpret classifications 
rather than simply repeating counts.

Relevant categories may include labels equivalent to:

- indexed;
- crawled but currently not indexed;
- discovered but currently not indexed;
- excluded by noindex;
- blocked by robots.txt;
- duplicate without user-selected canonical;
- alternate page with proper canonical;
- search engine selected a different canonical;
- page with redirect;
- not found;
- soft 404;
- server error;
- other crawl or indexing exclusions.

The exact labels may change over time.

Analyze the actual supplied report.

For each classification determine:

- whether the exclusion is intentional;
- whether affected URLs share a template;
- whether counts are growing;
- whether valuable URLs are affected;
- whether sitemap URLs are affected;
- whether canonical signals conflict;
- whether internal linking contributes;
- whether content quality or duplication may contribute.

Do not interpret every excluded URL as an SEO problem.

A healthy site can intentionally exclude large numbers of low-value or 
duplicate URLs.

4. Analyze "Crawled, Currently Not Indexed"

Treat this as an index-selection problem first, not automatically as a crawl 
problem.

Investigate patterns such as:

- weak or thin content;
- near duplicates;
- templated pages;
- substantially overlapping pages;
- soft-404 characteristics;
- low internal importance;
- weak unique value;
- duplicate product or location pages;
- generated URLs;
- outdated pages;
- conflicting canonicals;
- poor rendering;
- content not present in rendered output;
- unexpected status behavior;
- low-quality URL clusters.

Cross-reference:

- content similarity;
- internal links;
- crawl depth;
- sitemap inclusion;
- canonical target;
- page type;
- publication patterns;
- rendered content.

Do not prescribe repeated resubmission as the primary fix when the underlying 
page does not justify indexing.

5. Analyze "Discovered, Currently Not Indexed"

Determine why discovered URLs may not be receiving timely crawls.

Investigate:

- very large URL inventories;
- crawl traps;
- parameter explosion;
- faceted navigation;
- low internal importance;
- deep crawl depth;
- weak server performance;
- repeated errors;
- many low-value URLs;
- sitemap bloat;
- rapid generation of low-value URLs;
- crawler-resource competition;
- poor site architecture;
- duplicate URL discovery.

Do not automatically conclude that the site has a formal "crawl budget issue."

Determine whether actual evidence supports inefficient crawler allocation.

6. Analyze Crawl Efficiency

Crawl efficiency means directing crawler activity toward valuable resources 
while reducing unnecessary requests to low-value URL variants.

Look for crawler waste caused by:

- parameter combinations;
- faceted navigation;
- sorting URLs;
- calendar traps;
- infinite navigation;
- session IDs;
- tracking parameters;
- duplicate protocol or host variants;
- case-sensitive duplicates;
- trailing-slash duplicates;
- print pages;
- internal search pages;
- empty pagination;
- malformed relative URLs;
- infinite redirects;
- duplicate category paths;
- alternate URLs generated by scripts;
- unnecessary feed or endpoint URLs.

Quantify waste only when sufficient crawl or log data exists.

7. Crawl Budget Assessment

Use the term "crawl budget" carefully.

Do not assume every website is crawl-budget constrained.

Crawl-budget analysis is most useful when sites have characteristics such as:

- very large URL inventories;
- rapidly changing content;
- large ecommerce catalogs;
- extensive faceted navigation;
- millions of generated URLs;
- substantial duplicate discovery;
- high-frequency publishing;
- significant server limitations.

Distinguish:

Crawl Demand 
How much the crawler appears to want to revisit URLs.

Host Capacity / Crawl Capacity 
How much crawling the infrastructure can tolerate reliably.

Crawl Efficiency 
How much crawler activity reaches strategically useful URLs.

The absence of indexing does not prove insufficient crawl budget.

8. Server Log Analysis

When logs are available, use actual crawler requests to understand behavior.

Analyze:

- verified crawler traffic where possible;
- request counts;
- request frequency;
- directories crawled;
- URL patterns crawled;
- status-code distribution;
- redirect requests;
- parameter crawling;
- noncanonical crawling;
- orphan-page crawling;
- bot activity over time;
- crawl depth versus crawl frequency;
- important pages not receiving crawler requests;
- low-value URLs receiving disproportionate requests;
- 5xx/429 patterns;
- response latency.

Do not trust user-agent strings alone when bot authenticity matters.

Use appropriate verification methods or classify the crawler identity as 
unverified.

9. Analyze HTTP Status Codes

2xx

Confirm that successful responses contain meaningful intended content.

Watch for:

- blank 200 pages;
- error templates returning 200;
- removed products returning 200;
- empty search results returning 200;
- blocked content returning 200;
- login/error content returned instead of the expected page.

3xx

Analyze:

- redirect chains;
- redirect loops;
- temporary versus permanent behavior;
- internal links pointing to redirects;
- sitemap URLs that redirect;
- canonical targets that redirect;
- mass migration behavior.

Prefer direct internal links to the final canonical destination.

4xx

Distinguish intentionally removed URLs from broken internal architecture.

Investigate:

- internally linked 404s;
- sitemap 404s;
- backlinks to removed URLs;
- mistyped generated URLs;
- expired inventory;
- deleted content;
- broken pagination.

Use 404 or 410 appropriately according to the site's actual removal behavior.

Do not redirect every removed URL to the homepage.

5xx

Treat recurring server failures affecting crawler access as potentially high 
severity.

Analyze patterns by:

- template;
- server;
- time;
- directory;
- crawler;
- request rate.

429

Investigate rate limiting when legitimate search crawlers are affected.

Determine whether:

- CDN rules;
- WAF rules;
- application throttling;
- infrastructure limits

are unnecessarily restricting crawler access.

10. Soft 404 Analysis

Identify pages that return successful status codes but appear functionally 
missing or valueless.

Potential patterns:

- "product not found";
- empty location pages;
- zero-result categories;
- empty profiles;
- deleted content with a generic message;
- thin autogenerated pages;
- pages redirecting conceptually to unrelated destinations.

Determine whether the correct fix is:

- improve the content;
- consolidate;
- return a genuine 404/410;
- redirect to a genuinely equivalent replacement.

11. Robots.txt Analysis

Parse rules according to relevant crawler/user-agent context.

Inspect:

- User-agent;
- Disallow;
- Allow;
- sitemap declarations;
- wildcard patterns;
- end anchors where supported;
- conflicting user-agent groups;
- environment-specific rules.

Identify accidental blocking of:

- important pages;
- CSS;
- JavaScript;
- API resources needed for rendering;
- localized pages;
- product sections;
- media required for understanding.

Also identify unnecessary crawler access to low-value patterns when robots 
control is appropriate.

Critical Robots Principle

Do not confuse crawl blocking with deindexing.

Blocking a URL with robots.txt prevents or restricts crawling.

It should not be treated as a reliable equivalent of an index-removal 
directive.

If a crawler cannot access a page, it may also be unable to observe page-level 
directives such as noindex.

Consider the desired outcome before recommending robots blocking.

12. Meta Robots and X-Robots-Tag Analysis

Inspect directives such as:

- index/noindex;
- follow/nofollow;
- noarchive-like controls where applicable;
- snippet controls;
- image-related controls.

Check both:

- HTML meta robots;
- HTTP X-Robots-Tag.

Identify conflicts between:

- meta directives;
- HTTP directives;
- robots.txt;
- canonical tags;
- sitemaps.

Do not use nofollow as a substitute for controlling indexation.

13. Sitemap Analysis

Analyze both sitemap indexes and child sitemaps.

A high-quality XML sitemap should primarily contain URLs that the site wants 
search engines to crawl and consider for indexing.

Check for:

- non-200 URLs;
- redirects;
- 404/410 URLs;
- 5xx URLs;
- noindex URLs;
- robots-blocked URLs;
- noncanonical URLs;
- duplicate URLs;
- parameter variants;
- staging URLs;
- incorrect hosts;
- HTTP URLs on HTTPS sites;
- malformed entries;
- excessive sitemap sizes;
- obsolete sitemaps;
- empty sitemaps;
- incorrect sitemap nesting.

Evaluate whether sitemap segmentation is useful.

Possible segmentation dimensions include:

- page type;
- language;
- country;
- product category;
- freshness;
- content type.

Segmentation should help diagnosis and management rather than create 
unnecessary complexity.

14. Sitemap Freshness and lastmod

When lastmod values exist, determine whether they reflect meaningful content 
changes rather than simply being regenerated on every request or deployment.

Do not recommend artificial freshness signals.

Investigate sitewide identical timestamps or implausibly frequent changes when 
data permits.

15. Canonicalization Analysis

Treat rel=canonical as one canonicalization signal rather than an absolute 
command.

Inspect:

- self-referencing canonicals;
- cross-page canonicals;
- canonical targets;
- canonical chains;
- canonical targets returning errors;
- canonical targets redirecting;
- canonicals to blocked URLs;
- canonicals to noindex URLs;
- canonicals to different language versions;
- canonical differences between rendered and source HTML;
- HTTP header canonicals where applicable.

Cross-reference canonical hints with:

- redirects;
- internal links;
- XML sitemaps;
- duplicate content;
- hreflang;
- external links when available.

The strongest implementation gives search engines consistent signals.

16. Search-Engine-Selected Canonical Conflicts

When evidence indicates that a search engine chose a different canonical from 
the site's preferred canonical, investigate:

- content similarity;
- internal link dominance;
- inconsistent redirects;
- sitemap signals;
- URL variants;
- parameter duplication;
- weak unique content;
- hostname/protocol differences;
- canonical chains;
- hreflang errors;
- duplicate templates.

Do not respond by merely re-adding the canonical tag if the broader signals 
contradict it.

17. Duplicate URL Analysis

Identify duplication caused by:

- parameters;
- tracking IDs;
- sorting;
- filtering;
- pagination;
- uppercase/lowercase paths;
- slash variants;
- HTTP/HTTPS;
- www/non-www;
- session IDs;
- alternate taxonomy paths;
- duplicate categories;
- printer versions;
- syndication;
- duplicate product variants;
- search pages.

Determine the correct control mechanism based on the cause.

Possible solutions include:

- redirect;
- canonicalization;
- internal-link cleanup;
- parameter-generation prevention;
- sitemap cleanup;
- robots rules;
- noindex;
- application-level routing changes;
- consolidation.

Do not use one solution mechanically for every duplicate pattern.

18. Faceted Navigation

Treat faceted navigation as both a crawl-efficiency and search-demand problem.

Identify:

- filter combinations;
- sort parameters;
- multi-select filters;
- near-infinite combinations;
- zero-result facets;
- low-demand combinations;
- high-value searchable combinations.

Determine which facets should be:

- indexable landing pages;
- canonicalized;
- blocked from crawling;
- noindexed;
- prevented from generating crawlable URLs;
- internally linked selectively.

Do not remove all faceted URLs automatically.

Some combinations can represent legitimate search demand.

19. URL Parameter Analysis

Classify parameter purpose.

Examples:

- tracking;
- sorting;
- filtering;
- pagination;
- session;
- search;
- view mode;
- referral;
- state management.

Identify whether parameters change:

- content materially;
- ordering only;
- presentation only;
- analytics state only.

Recommend controls based on actual URL behavior.

20. Pagination

Analyze paginated series for:

- crawlable navigation;
- unique URLs;
- self-consistent canonicals;
- indexability strategy;
- internal links to deeper pages;
- orphaned deeper pages;
- empty pagination;
- endless pagination patterns.

Do not automatically canonicalize every paginated page to page one.

Determine whether deeper pages are necessary for content discovery.

21. Infinite Scroll and Load-More Interfaces

Verify whether content loaded dynamically is also discoverable through crawlable 
URLs and links where needed.

Inspect:

- real anchor elements;
- href destinations;
- paginated fallbacks;
- history-state routing;
- JavaScript-only click handlers;
- crawler-visible content.

A visually accessible interface can still have weak crawler discovery.

22. Internal Linking Analysis

Internal links communicate both discovery and relative importance.

Analyze:

- crawl depth;
- inlinks;
- link distribution;
- navigation;
- contextual links;
- breadcrumbs;
- related-content modules;
- category links;
- footer links;
- pagination links.

Identify:

- orphan pages;
- near-orphan pages;
- important pages buried too deeply;
- low-value URLs receiving excessive internal links;
- redirecting internal links;
- canonicalized URLs still linked extensively;
- 404 links;
- links generated only through unreliable JavaScript interactions.

Prioritize improving internal-link architecture for important pages rather than 
merely increasing total link counts.

23. Orphan Page Analysis

Do not label every URL absent from a crawl as a true orphan automatically.

Cross-reference with:

- XML sitemaps;
- analytics;
- Search Console;
- backlinks;
- server logs;
- known URL inventories.

Classify pages such as:

- true orphan;
- sitemap-only;
- externally discoverable;
- intentionally isolated;
- legacy orphan;
- generated orphan.

Determine whether valuable orphan pages should be integrated into site 
architecture or intentionally removed.

24. Crawl Depth

Use crawl depth as a diagnostic signal, not an absolute ranking rule.

Identify important pages that require unnecessarily long click paths.

Analyze depth together with:

- internal links;
- page type;
- site hierarchy;
- business importance;
- crawl frequency;
- search performance.

25. JavaScript Rendering and Indexability

When a site relies on JavaScript, determine whether essential content and links 
exist reliably in rendered output.

Inspect:

- server-rendered HTML;
- client-rendered HTML;
- hydration;
- API calls;
- blocked JS resources;
- lazy-loaded text;
- click-dependent links;
- route transitions;
- dynamic canonicals;
- dynamic robots directives;
- dynamic metadata.

Detect cases where:

- canonical appears only after rendering;
- noindex changes after hydration;
- content differs substantially between source and rendered HTML;
- links lack crawlable href values;
- API failure produces thin pages;
- client routes return problematic server responses.

Recommend fixes at the actual rendering layer.

26. Rendering Resource Accessibility

If page understanding depends on external resources, inspect whether relevant:

- CSS;
- JavaScript;
- APIs;
- image resources

are accessible to crawlers when necessary.

Do not assume every blocked script harms indexing.

Determine whether the blocked resource is actually required to render or 
understand important content.

27. SPA and Client-Side Routing

For single-page applications, analyze:

- server responses for deep URLs;
- route fallback behavior;
- canonical output;
- status codes;
- metadata;
- internal anchor behavior;
- hydration;
- direct navigation;
- error routes.

A client-side route that visually works can still return technically misleading 
server behavior.

28. Content Quality and Index Selection

When technically indexable URLs remain unindexed, evaluate content patterns.

Look for:

- thin pages;
- near duplicates;
- templated location pages;
- programmatic pages with minimal differentiation;
- empty category pages;
- product variants with identical information;
- outdated content;
- doorway-like pages;
- low-information tag archives;
- generated search pages;
- repeated boilerplate overwhelming unique content.

Do not label content "low quality" without evidence.

Describe the observed pattern that may reduce index-worthiness.

29. Low-Value URL Inventory

Identify URL classes whose indexing provides little search value.

Examples may include:

- empty tags;
- internal search results;
- duplicate filters;
- thin archives;
- utility pages;
- account pages;
- parameter duplicates;
- session URLs;
- preview URLs.

Determine the intended treatment for each class.

Possible actions:

- keep indexed;
- consolidate;
- noindex;
- block crawling;
- remove;
- redirect;
- stop generating;
- remove from sitemap;
- reduce internal links.

Select controls according to the actual objective.

30. Search Architecture

Assess whether site architecture reflects the business and content hierarchy.

Determine whether important categories, products, services, locations, or topic 
hubs are:

- easily discoverable;
- internally connected;
- sufficiently shallow;
- linked from relevant parent pages.

Identify architecture that causes crawler effort to be spread across 
low-priority pages while valuable pages remain weakly linked.

31. HTTP/HTTPS and Host Consistency

Inspect duplication between:

- HTTP and HTTPS;
- www and non-www;
- alternate domains;
- subdomains;
- trailing-slash variants;
- mixed capitalization.

Check:

- redirects;
- canonicals;
- sitemaps;
- internal links;
- hreflang references.

Prefer one coherent canonical URL pattern.

32. Hreflang Interactions

When internationalization exists, check whether hreflang creates crawl or 
canonical conflicts.

Inspect:

- return links;
- canonical compatibility;
- language/region URLs;
- nonindexable hreflang targets;
- redirected targets;
- incorrect language pairings;
- broken URLs.

Do not perform a full international SEO audit unless relevant to the task.

33. Migration and URL Change Analysis

For migrations, analyze:

- legacy-to-new redirects;
- redirect chains;
- missed mappings;
- canonical changes;
- sitemap updates;
- internal-link updates;
- orphaned new pages;
- old URLs still discoverable;
- host/protocol changes.

Prefer direct one-hop redirects to genuine equivalents where possible.

34. Crawl Traps

Actively detect crawl traps such as:

- infinite calendars;
- endless pagination;
- recursive parameters;
- sort/filter permutations;
- session URLs;
- dynamically generated empty pages;
- malformed link generation;
- auto-generated date paths;
- infinite internal-search URLs.

Treat severe crawl traps as high priority on large sites.

35. Search Engine Crawl Controls

When recommending a control, state what it actually accomplishes.

Distinguish among:

- robots.txt;
- noindex;
- canonical;
- redirect;
- HTTP status;
- sitemap inclusion;
- internal-link changes;
- URL-generation changes.

Do not use these controls interchangeably.

36. AI Search and Retrieval Accessibility

Assess AI visibility conservatively.

Technical SEO controls that improve ordinary crawler accessibility can also 
improve the availability of content to systems that depend on web crawling, 
retrieval, or indexed corpora.

Evaluate:

- whether important content is crawlable;
- whether content exists in retrievable HTML;
- whether important pages are indexable;
- whether canonical identity is clear;
- whether the site architecture exposes authoritative pages;
- whether content is internally connected;
- whether duplicate URLs obscure the preferred source;
- whether blocked resources prevent meaningful extraction.

Do not claim that improving crawlability guarantees inclusion in:

- AI-generated answers;
- AI Overviews;
- LLM citations;
- answer-engine responses.

Different systems may use different crawlers, indexes, licensing arrangements, 
and retrieval mechanisms.

Cross-Source Diagnosis

Whenever multiple datasets exist, cross-reference them.

Examples:

GSC + Crawl

Compare unindexed URLs with:

- status code;
- canonical;
- noindex;
- depth;
- internal links;
- sitemap inclusion.

GSC + Sitemap

Determine whether URLs submitted for indexing are:

- indexed;
- excluded intentionally;
- redirected;
- canonicalized;
- low value.

Crawl + Logs

Compare what can be crawled with what search bots actually crawl.

Sitemap + Logs

Identify submitted important URLs receiving little or no observed crawler 
activity.

Internal Links + Logs

Determine whether strongly linked URLs are crawled more frequently than weakly 
linked pages.

Canonicals + Internal Links

Detect when the site declares one canonical but links predominantly to another 
variant.

Cross-source agreement increases confidence.

Root Cause Analysis

Do not stop at symptoms.

For each meaningful issue, determine the likely layer causing it.

Possible root-cause layers include:

- infrastructure;
- CDN;
- WAF;
- server;
- application;
- framework;
- routing;
- CMS;
- plugin;
- template;
- database;
- navigation;
- editorial process;
- sitemap generator;
- JavaScript rendering;
- URL architecture.

Example:

Symptom: 
Thousands of redirected URLs in XML sitemaps.

Weak recommendation: 
Remove redirects from the sitemap.

Root-cause recommendation: 
Update the sitemap-generation function so it exports only current canonical 
200-status URLs, then regenerate all affected sitemap files and remove legacy 
redirecting paths from internal links.

Severity Model

Critical

Issues capable of preventing major sections or the entire site from being 
accessed or indexed.

Examples:

- sitewide noindex;
- production site blocked by robots;
- widespread 5xx;
- canonicalization of most pages to the wrong destination;
- catastrophic redirect loops;
- inaccessible rendering of core content.

High

Major problems affecting important URL classes or causing substantial crawl 
waste.

Examples:

- high-value pages not indexable;
- large crawl traps;
- major canonical conflicts;
- important pages omitted from architecture;
- widespread sitemap contamination;
- major duplicate generation;
- persistent server instability.

Medium

Issues with meaningful but limited impact.

Examples:

- redirect chains;
- weak internal linking;
- moderate orphan-page patterns;
- unnecessary parameter crawling;
- template-level sitemap inconsistencies.

Low

Minor inefficiencies or cleanup tasks.

Examples:

- isolated redirected internal links;
- small numbers of obsolete sitemap URLs;
- limited optional crawl optimizations.

Assign severity according to affected business value and scale, not issue name 
alone.

Prioritization Model

Prioritize using:

- number of valuable URLs affected;
- business importance;
- indexing impact;
- crawl-efficiency impact;
- severity;
- sitewide/template scope;
- implementation effort;
- confidence;
- reversibility;
- expected outcome.

Prefer fixing template-level root causes over manually correcting thousands of 
individual URLs.

Optimization Workflow

After diagnosis, optimize in roughly this order when applicable:

1. Remove critical crawl/index blockers.
2. Restore correct HTTP responses.
3. Fix severe robots or noindex mistakes.
4. Fix canonical conflicts.
5. Stop major crawl traps.
6. Improve sitemap quality.
7. Repair broken internal discovery paths.
8. Consolidate duplicate URL generation.
9. Improve important-page internal linking.
10. Resolve rendering barriers.
11. Improve index-worthiness of valuable unindexed pages.
12. Remove or control low-value indexable inventory.
13. Improve ongoing crawl monitoring.

Do not follow this order mechanically if the evidence supports a different 
priority.

Output Structure

Adapt the report to the invoking prompt.

Do not output empty sections.

Executive Summary

Summarize:

- overall crawlability;
- overall indexability;
- crawl-efficiency health;
- index-selection health;
- most serious technical issue;
- most serious architectural issue;
- most significant quick win;
- whether evidence supports a genuine crawl-budget concern.

Crawl and Indexability Scorecard

When sufficient evidence exists, summarize:
Area	Status	Evidence	Confidence	Priority
Discovery				
Crawlability				
Rendering				
Indexability				
Canonicalization				
XML Sitemaps				
Robots Controls				
Internal Linking				
Crawl Efficiency				
Index Selection				

Use qualitative statuses unless real quantitative data exists.

Key Findings

For every meaningful issue provide:
Issue	Severity	Evidence Status	Confidence	Evidence	Root Cause	Affected URLs / Pattern	Recommended Fix	Expected Outcome


Be specific.

Indexing Diagnosis

Explain which excluded URLs are:

- intentional and healthy;
- technically problematic;
- likely duplicate;
- low value;
- under-discovered;
- crawl constrained;
- uncertain.

When data permits, analyze major indexing-report classifications separately.

Crawl Efficiency Analysis

Identify:

- useful crawler activity;
- low-value crawl activity;
- crawl traps;
- duplicate discovery;
- parameter waste;
- redirects;
- error crawling;
- noncanonical crawling.

Do not quantify crawler waste without actual supporting data.

Crawl Budget Assessment

State one of:

- Evidence supports a meaningful crawl-budget constraint.
- Crawl efficiency issues exist, but a crawl-budget constraint is not proven.
- Available evidence does not indicate a meaningful crawl-budget issue.
- Insufficient evidence to assess crawl budget.

Explain why.

Sitemap Review

Assess:

- sitemap cleanliness;
- canonical URL inclusion;
- status-code quality;
- indexable URL ratio;
- freshness;
- sitemap segmentation;
- sitemap/indexing contradictions.

Robots and Index Directive Review

Assess:

- robots rules;
- noindex;
- X-Robots-Tag;
- crawler-specific rules;
- directive conflicts;
- accidental blocking.

Canonicalization Review

Identify:

- canonical conflicts;
- duplicate clusters;
- inconsistent signals;
- search-engine-selected canonical problems;
- protocol or hostname conflicts.

Internal Discovery and Architecture

Identify:

- orphan pages;
- deep important pages;
- weakly linked commercial pages;
- overlinked low-value URLs;
- broken links;
- redirected internal links;
- crawlable navigation issues.

Rendering Review

When relevant, cover:

- server-rendered content;
- JavaScript rendering;
- client-side links;
- hydration;
- dynamic metadata;
- blocked resources;
- SPA routing.

URL Pattern Findings

Group issues by patterns rather than listing every affected URL when many URLs 
share one root cause.

Example:

/products/?sort=*

rather than repeating hundreds of individual URLs.

Include sample URLs where useful.

Search and AI Visibility Risks

Explain technical issues that may reduce:

- organic search discoverability;
- indexing;
- ranking eligibility;
- content retrieval;
- machine access.

Keep AI visibility claims appropriately qualified.

Immediate Fixes

Include high-impact, urgent actions.

Short-Term Fixes

Include improvements suitable after critical blockers are corrected.

Medium-Term Structural Improvements

Include architecture, platform, CMS, rendering, or URL-strategy changes.

Developer Implementation Notes

When implementation context exists, explain where fixes should occur.

Examples:

- router;
- server middleware;
- sitemap generator;
- CMS template;
- SEO component;
- CDN configuration;
- robots generation;
- pagination component.

Prefer system-level fixes over manual URL-by-URL patches.

Validation Plan

For each major change, explain how to verify it.

Use explicit validation states:

- Verified — the check was completed and produced the expected result;
- Failed — the check was completed and did not produce the expected result;
- Not Checked — verification was not performed;
- Monitoring Required — implementation checks passed but search-engine 
- recrawling, reprocessing, or index-selection evidence is still pending.

Where useful, report validation as:
Change or Check	Validation Status	Evidence or Result	Remaining Uncertainty	Next Step


Possible checks:

- recrawl affected URLs;
- inspect rendered HTML;
- validate robots rules;
- fetch sitemap;
- verify HTTP headers;
- verify canonical;
- inspect logs;
- compare GSC indexing classifications after recrawl/reprocessing;
- test representative template URLs.

Do not promise how quickly a search engine will recrawl or reindex pages.

Prioritized Action Plan

Finish with an ordered action plan.

Each action should include:

1. exact change;
2. affected pattern or system;
3. responsible layer where identifiable;
4. priority;
5. expected technical outcome;
6. verification method.

Quality Rules

Be diagnostic rather than descriptive.

Do not repeat metrics without interpretation.

Do not call every exclusion an error.

Do not assume an unindexed URL should be indexed.

Do not assume more indexed pages is always better.

Do not use "crawl budget" as a generic explanation for indexing problems.

Do not confuse discoverability with crawlability.

Do not confuse crawlability with indexability.

Do not confuse indexability with actual indexing.

Do not confuse canonicalization with guaranteed deindexing.

Do not confuse robots blocking with noindex.

Do not recommend adding blocked URLs to sitemaps as a workaround.

Do not include redirects, noindex URLs, or obvious noncanonical duplicates in 
sitemaps unless a specific justified workflow requires it.

Do not recommend repeated manual indexing requests as a substitute for fixing 
systemic problems.

Do not recommend blocking all parameters without understanding their function.

Do not assume every faceted URL is low value.

Do not canonicalize every pagination URL to page one automatically.

Do not redirect unrelated removed URLs to the homepage.

Do not diagnose content quality from status codes alone.

Do not fabricate search-engine crawler behavior.

Do not claim AI-search visibility guarantees.

Prefer fixing URL generation over repeatedly cleaning generated bad URLs.

Prefer fixing shared templates over editing large numbers of pages manually.

Prefer coherent technical signals across:

- redirects;
- canonicals;
- internal links;
- sitemaps;
- index directives.

The final analysis should make clear:

- which important URLs are discoverable;
- which can actually be crawled;
- which can be rendered;
- which are technically indexable;
- which are likely index-worthy;
- which are actually indexed according to available evidence;
- where crawler activity is being wasted;
- which exclusions are intentional;
- which exclusions are harmful;
- which canonical signals conflict;
- which URL patterns create crawl traps;
- which architectural patterns weaken discovery;
- whether crawl-budget concerns are real or merely assumed;
- what developers or SEOs should fix first;
- how each fix should be validated.
