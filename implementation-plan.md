# Academic Website Architecture and Implementation Plan

## Website Architecture

- Home: headshot placeholder, academic identity, research interests, biography, featured research, recent news, research metrics, and quick links.
- Research: published papers, forthcoming papers, working papers, and work in progress, with abstract toggles, journal metadata, PDF buttons, and citation blocks.
- CV: education, employment, publications, presentations, awards, grants, teaching, and service, with PDF download and print support.
- Teaching: courses taught, TA experience, teaching philosophy, and course materials.
- Projects: current research projects organized by research question, data sources, methodology, and status.
- Professional Activities: editorial experience, peer review, conferences, and memberships.
- Contact: university email, Google Scholar placeholder, LinkedIn placeholder, office location, and contact form.

## Design System

- Philosophy: minimalist, research-focused, committee-friendly, and inspired by Harvard/MIT/Chicago economics pages.
- Typography: Georgia for headings and academic prose; Arial/Helvetica for navigation, metadata, and interface text.
- Palette: white background, near-black text, warm burgundy academic accent, light gray rules, and subtle off-white section surfaces.
- Layout: maximum width of 1120px, generous margins, strong typographic hierarchy, restrained borders, no decorative graphics.
- Components: header navigation, headshot placeholder, paper records, project records, CV entries, native HTML details toggles, metric blocks, and accessible form fields.

## Page Layouts

- Home uses a two-column academic profile layout on desktop and a single-column layout on mobile.
- Research uses stacked paper entries grouped by publication status.
- CV uses printable long-form sections suited to hiring committee review.
- Teaching and activities use two-column organization where scanning matters.
- Projects use full-width records to keep research questions and methodology readable.
- Contact uses a two-column information/form layout.

## SEO and Accessibility

- Each page includes descriptive titles and meta descriptions.
- Semantic HTML landmarks are used for header, navigation, main content, sections, articles, and footer.
- Native details/summary controls support keyboard-accessible abstract toggles.
- Links and controls include visible focus states.
- Color contrast is high and text remains readable on mobile.

## Performance

- No external dependencies.
- No JavaScript framework.
- System fonts avoid font loading delays.
- Static HTML/CSS keeps page speed high and hosting simple.

## Implementation Steps

1. Replace placeholder paper titles, coauthors, abstracts, journal details, and PDF links with verified publication data.
2. Add a final professional headshot image and replace the placeholder block on the home page.
3. Upload the finalized PDF CV as `cv.pdf`.
4. Replace Google Scholar and LinkedIn placeholders with profile URLs.
5. Add analytics only if needed, using a privacy-preserving lightweight option.
6. Deploy to a university web server, GitHub Pages, Netlify, or another static hosting provider.
