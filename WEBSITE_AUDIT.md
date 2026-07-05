# Audit and redesign rationale for alexiosevich.com

## Overall assessment

The current site contains unusually rich material: research, mentoring, students, postdocs, collaborators, undergraduate programs, talks, media, poetry, and professional service. The main weakness is not lack of substance. It is that the most important substance is difficult to identify quickly.

The redesigned front layer keeps the site static and simple. It uses plain HTML, one CSS file, no JavaScript, no framework, no database, no web fonts, and no build system.

## Highest-impact changes

1. The homepage now begins with a clear professional identity and research statement rather than making visitors infer the purpose of the site from a photo, quotation, and link list.

2. The main navigation is reduced to six stable categories: Research, People & Mentoring, Programs & Outreach, Media, CV, and Contact.

3. The current StemForAll program remains prominent, but it no longer displaces the core professional introduction.

4. Research is presented as four connected themes rather than as a directory of links.

5. Mentoring, students, postdocs, collaborators, and undergraduate research are brought together under one coherent heading.

6. Time-sensitive course and schedule links are separated from evergreen mentoring content.

7. The site now has a consistent header, footer, typography, spacing system, mobile layout, keyboard focus states, descriptive page titles, meta descriptions, and semantic headings.

8. The Hirsh Glick quotation and the photograph with Mason are retained, but placed within a stronger professional hierarchy.

## Content problems that should be corrected in the legacy pages

The redesign does not rewrite the very large CV, student, postdoc, collaborator, and StemForAll archive pages. Before those pages are visually modernized, their content should be cleaned.

### About page

The current page contains small but visible errors such as “Alex iosevich,” “postodoctoral,” and “Another passion of mine in vertical integration.” The replacement `about` file corrects these and gives the page a clearer structure.

### Ph.D. student page

The introductory statistics and the statistics at the bottom do not agree. The page begins with 17/28 and 10/22, ends with 18/30 and 22/30, and lists 38 people. Several entries contain copied names, incorrect years, outdated positions, or typographical errors. Examples include the Steven Senger entry beginning with “David,” the Shashank Chorge entry beginning with “Donggeun,” and inconsistent graduation dates.

Recommendation: create a small spreadsheet with one row per student and columns for degree year, co-adviser, area, first position, current position, postdoc indicator, and academic/industry category. Generate the page from that single source of truth, or at minimum use it to verify all counts.

### Postdoc page

The page lists 15 postdocs but reports a statistic with denominator 13. Several current positions and spellings should be checked.

### Collaborator page

The introduction says both 204 and 205 collaborators. The list also contains numerous spelling, affiliation, and capitalization inconsistencies. The color coding for five or ten papers should be supplemented with text or symbols so the distinction is not conveyed by color alone.

### StemForAll 2026 page

The page says it was last updated in December 2025, refers once to “StemForAll2025” in a 2026 location paragraph, contains duplicate participant names, and has several grammar and spelling errors. Because this page is currently promoted from the homepage, it should receive priority proofreading.

### CV

The web CV is exceptionally complete but very long. It mixes a short professional profile, current material, historical lists, and detailed archival records in a single 1,700-line page. It also contains duplicate entries and many old job titles that are no longer current.

Recommendation: retain the complete CV as an archive, but add a compact contents panel at the top and create a separate two-page PDF or concise web biography for visitors who do not need the full record.

## Files in this package

- `index.html`: replacement homepage
- `style.css`: the only stylesheet
- `about`: replacement for the current extensionless About page
- `researchpage.html`: replacement research hub
- `mentoringandteaching`: replacement extensionless people and mentoring hub
- `dissemination`: replacement extensionless programs and outreach hub
- `media`: replacement extensionless media page
- `editorialwork.html`: replacement editorial service page

The design deliberately links to the existing deep archive pages rather than forcing an immediate migration of the entire site.
