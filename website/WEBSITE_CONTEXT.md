# Website Context

## Purpose

The website supports the event before and during each yearly tournament. The final event and website name has not been selected; use `[Event Name]` as a placeholder until it is decided. The website should serve two primary user groups: students and participating companies.

The platform has two main purposes:

1. Handle event registration and participation details.
2. Help motivated students and Stavanger-area employers discover and connect with each other.

The experience should feel professional but informal, reflecting an event focused on recruitment, community, networking, and fun.

## User Types

### Students

Students are primarily studying business, finance, economics, or related subjects. They are based in Stavanger, study elsewhere but come from the Stavanger area, or are interested in working in the region.

Students should be able to:

- Create and maintain a personal profile.
- Upload a profile photo.
- Enter their university or educational institution.
- Enter their field of study.
- Enter their current year of study.
- Enter their current study location.
- Enter where they are originally from.
- Add professional and academic areas of interest.
- Add skills, work experience, and other relevant experience.
- Enter their golf handicap.
- Upload a CV and optional supporting documents.
- Control which documents are shared with verified companies.
- View participating company profiles and relevant opportunities.
- Register for the tournament.
- Manage participation details.

### Companies

Companies are initially expected to include banks, finance companies, consultancies, and other relevant Stavanger employers.

Companies should be able to:

- Create and maintain a company profile.
- Upload a company logo and relevant company image.
- Present company information, industry, employees, roles, and opportunities.
- Select up to five core qualities they look for in students and prospective employees.
- Select qualities from suggested options or add custom qualities.
- View and search student profiles.
- Filter students using relevant structured profile information.
- Open student profiles.
- Privately mark participating students as favorites.
- Access CVs and documents that students have deliberately shared with verified companies.
- Manage the company representatives participating in the tournament.

### Company Representatives

Each participating company representative should have a personal profile containing:

- Full name.
- Role or job title.
- Profile photo.
- Golf handicap.
- Associated company.

Golf handicap is tournament information used for scoring, administration, and team allocation. It must not be used for recruitment matching.

## Profile Fields

### Student Profile

The student profile should contain at least:

| Field | Purpose | Visibility decision |
|---|---|---|
| Full name | Identity and networking | To be decided |
| Profile photo | Recognition and networking | To be decided |
| Field of study | Recruitment and matching | Company-visible |
| Current year of study | Recruitment and matching | Company-visible |
| University/institution | Education context | Company-visible |
| Study location | Regional context | Company-visible |
| Place of origin | Stavanger connection and networking | Company-visible; student visibility to be decided |
| Areas of interest | Discovery and matching | Company-visible |
| Skills and experience | Recruitment | Company-visible |
| Golf handicap | Tournament administration | Restricted to relevant event users and organizers |
| CV | Recruitment | Verified companies only, with student consent |
| Supporting documents | Recruitment | Verified companies only, with student consent |

### Company Profile

The company profile should contain at least:

- Company name.
- Logo.
- Relevant company image.
- Industry.
- Description.
- Stavanger presence or regional connection.
- Relevant roles, internships, graduate positions, or other opportunities.
- Participating company representatives.
- Up to five prioritized core qualities.
- Sponsorship or event-partner status where relevant.

## Core Qualities

Companies can select up to five qualities they prioritize when meeting or recruiting students. The interface should offer suggestions while allowing companies to create their own.

Initial suggested qualities include:

- Analytical.
- Collaborative.
- Curious.
- Initiative-taking.
- Structured.
- Commercially minded.
- Adaptable.
- Clear communicator.
- Responsible.
- Relationship-oriented.

Suggested and custom qualities should use the same structured data format. This allows qualities to support search, filters, profile discovery, and future matching features.

Students should be able to see the five qualities each company prioritizes. The platform should not automatically claim that a student possesses a quality unless that information is explicitly supported by the student's profile or a future, transparent matching method.

## Discovery and Networking

Students should be able to browse participating companies and understand:

- What the company does.
- Which roles or opportunities may be relevant.
- Which representatives are attending.
- Which qualities the company prioritizes.

Verified company users should be able to browse and search students using appropriate fields such as:

- Field of study.
- Year of study.
- Study location.
- Areas of interest.
- Skills and experience.
- Regional connection.

The exact filters and whether students can browse other student profiles remain open decisions.

Company favorites must be anonymous to students and other companies. A favorite should only act as a preference signal for team allocation, increasing the chance that a company representative and the student are placed on the same scramble team. It must not guarantee a pairing, expose recruitment interest, or override tournament constraints such as team size and handicap balance. The organizer's access to favorite data and the exact weighting remain to be decided.

## Event Features

The website should eventually support:

- Student registration and payment.
- Company and representative registration.
- Event capacity and waiting list management.
- Golf handicap collection.
- Team allocation involving students and company representatives.
- Participant updates and practical event information.
- Dinner and afterparty attendance details.
- Dietary requirements.
- Administrative exports for organizers.

Tournament scoring, live results, or integration with golf software may be added later. The scoring method and any external system have not yet been selected.

## Documents and Access Control

- Public visitors must never have access to private student documents.
- Student documents must only be accessible to authenticated and authorized company users.
- Company accounts must be verified before document access is enabled.
- Students must deliberately choose which documents to share.
- Students must be told clearly who can access shared documents and for what purpose.
- Students must be able to withdraw access and delete uploaded documents.
- Document access should be limited to a defined recruitment purpose and period.
- Access to student data must not be sold as unrestricted sponsor access.
- Organizers should have only the access required for administration and support.

## Privacy and Security

The platform will hold personal information and recruitment documents. It therefore requires:

- Clear privacy notices and consent records.
- Role-based access control for students, company users, company representatives, organizers, and public visitors.
- Verified company accounts.
- Secure authentication and account recovery.
- Secure private document storage.
- Time-limited document links rather than public file URLs.
- Retention rules for accounts, profiles, applications, and documents.
- Account and document deletion processes.
- Logging of sensitive document access where appropriate.
- A process for reporting inappropriate access or profile content.
- Data minimization: only collect information required for the event or stated networking purpose.

Detailed privacy, retention, and consent rules must be settled before implementation and reviewed against applicable Norwegian and European data-protection requirements.

## Initial Product Scope

A sensible first release should focus on:

1. Student and company registration.
2. Verified role-based accounts.
3. Student, company, and representative profiles.
4. Company browsing for students.
5. Student browsing for verified companies.
6. Private, consent-based CV upload and access.
7. Event registration and payment status.
8. Organizer administration and exports.
9. Anonymous company favorites used as a weighted input to scramble team allocation.

Advanced automated matching, live scoring, messaging, and year-round job listings can be considered after the core workflow is proven.

## Confirmed Product Decisions

1. **Working name:** Use `[Event Name]` as a placeholder. The final name will be selected later.
2. **Primary student action:** Create a student profile, explore participating companies, and understand what each company does and looks for in students.
3. **Primary company action:** Browse participating students and privately favorite interesting candidates. Favorites anonymously increase the chance of sharing a scramble team.
4. **First-release scope:** Not yet decided. The initial product scope above is a working proposal, not a final commitment.
5. **Active period:** The website only needs to be operational before and during the tournament. Exact opening and closing dates remain to be decided.
6. **Yearly events and archive:** Each tournament should have its own event page. Information from previous tournaments should be retained in a historical archive and database where legally permitted.
7. **Active tournaments:** The platform only needs to support one active tournament at a time for now.
8. **Public information:** Visitors without an account should be able to see general event information, the schedule, participating companies, sponsors, and appropriate historical event information. Student profiles, private participant details, favorites, CVs, and supporting documents must never be public.
9. **Languages:** Users should be able to switch between Norwegian and English using a standard language selector. User-provided profile content does not need automatic translation in the first release.
10. **Accounts between events:** Profiles and accounts should be retained for reuse in later tournaments. Returning users should review and confirm their information before registering for a new event.

Historical participant data must not automatically become a public participant directory. Retention of personal profiles, CVs, documents, and company access must be covered by clear consent, retention periods, deletion rights, and applicable data-protection requirements. Public historical pages should use an explicitly approved subset of event information.

## Confirmed Design Direction

1. **Brand material:** No logo, color palette, typography, or other visual identity exists yet. These should be created after the final event name is selected.
2. **Visual balance:** The identity should combine golf and professional networking, weighted approximately 60% toward golf and 40% toward networking.
3. **Tone:** The website should feel fairly formal and credible while making it clear that the event is social and primarily intended to be fun.
4. **Visual reference:** Review [sologsving.no](https://sologsving.no/) and the `sologsving` Instagram account together with the organizer when design work begins. Use the website as functional inspiration for its event countdown, sponsor-logo strip, and partnership call to action. Do not copy its wording, layout, branding, imagery, or visual identity.
5. **Styles to avoid:** There is no specific prohibited style, but the result must not look generically AI-generated or "vibecoded." It should have a deliberate identity, consistent visual system, relevant content, and carefully designed responsive states.

Before a visual direction is selected, the AI design process must present several genuinely distinct color-palette options. Each option should include named color values, typography suggestions, accessibility considerations, and small examples showing the palette applied to relevant website components. The organizer must select or refine a direction before the complete interface is designed.

Initial palette options are documented in [COLOR_PALETTES.md](COLOR_PALETTES.md).

6. **Photography:** A future image gallery from Sola GK is expected to provide course imagery. The available images, formats, quality, and permitted uses must be confirmed before design begins. Additional event photography can be added after the first tournament.
7. **Image administration:** The organizer is responsible for approving and administering image use. This does not by itself transfer copyright or provide participant consent; the organizer must obtain appropriate licenses, photographer agreements, venue permission, and participant consent where required.
8. **Sponsor visibility:** Sponsors should appear on a dedicated sponsor page and in a visible section on the homepage. Inspired by the function on `sologsving.no`, the homepage should use a slowly moving horizontal sponsor-logo strip. The implementation must have its own layout and styling, support manual navigation, pause when appropriate, respect reduced-motion preferences, and keep every sponsor accessible without relying on animation.
9. **Dark mode:** Dark mode is not required.
10. **Accessibility:** No additional accessibility requirements have been identified beyond established good practice and the agreed WCAG baseline.
11. **Responsive design:** The website does not need to be mobile-first, but every core workflow must work well on both mobile and desktop. Event-day views should be especially easy to use on a phone.
12. **Event-day priorities:** Participants must be able to quickly find their start time, scramble team, starting hole, event program, results, and organizer contact information.

## Confirmed Navigation Decisions

1. **Primary sections:** Shared navigation should include Tournament, Program, Sponsors, Contact, and My Profile. Additional navigation should change according to whether the signed-in user is a student or company user.
2. **Dashboards:** Students and companies should have separate dashboards tailored to their tasks and available information.
3. **Shared pages:** Both user types should have access to Tournament, Program, Sponsors, Contact, and My Profile. The content and available actions within My Profile will be role-specific.
4. **Separate workflows:** Event information, registration, profile management, and discovery should be separate, clearly labeled workflows. This is a provisional decision and should be validated when wireframes are reviewed.
5. **Homepage states:** The homepage should change according to the event phase. Before registration it should show the event concept, date, venue, participating companies, and registration opening date. While registration is open it should prioritize registration and remaining capacity. When full it should show the waiting-list option and practical event information. After the tournament it should show results, approved photos, sponsors, and a link to the event archive. These are working recommendations.
6. **Student bookmarks:** Students should be able to privately save participating companies as favorites. Student favorites are for personal organization and must be kept separate from company favorites used by the team-allocation algorithm.
7. **Contact:** Direct messaging is not required. Companies and students can connect through approved contact details, email, LinkedIn, or in person at the event. Users must control whether their contact details are visible.
8. **Notifications:** Use a combination of in-app and external notifications. The recommended baseline is an in-app notification center plus email for registration, payment, profile, schedule, and team updates. SMS should be reserved for urgent or time-sensitive event-day changes. Exact triggers, consent, and opt-out rules remain to be approved.

Alternative notification models considered:

- **Minimal:** Email only, with critical information also visible on the dashboard. Lowest complexity and cost.
- **Balanced (recommended):** In-app notifications and email for normal updates, with SMS only for urgent event-day changes.
- **High-touch:** In-app, email, and SMS for most milestones. More immediate, but more expensive and more likely to feel intrusive.

## Homepage Features

### Event Countdown

The homepage should include a countdown to the tournament start, showing days, hours, minutes, and seconds. It should use the configured event date and time rather than hard-coded values. When the countdown reaches zero, it should be replaced by a relevant event-day state instead of displaying negative values or remaining at zero.

### Partnership Call to Action

The homepage and sponsor page should contain a visible partnership call to action. Use original, direct wording such as **Bli samarbeidspartner** rather than copying the reference website. The action should lead to the contact page or a future partnership enquiry form.

Supporting copy should briefly explain that companies can contribute through sponsorship, participant packages, prizes, stands, or other event collaboration. Final text will be written after the sponsorship packages are confirmed.

## Contact Page

A public Contact page is required. It should identify Marcus Grude Grodem as the organizer and provide:

- **Email:** [marcus.grude.grodem@gmail.com](mailto:marcus.grude.grodem@gmail.com)
- **Phone:** [+47 960 16 750](tel:+4796016750)

The email address and telephone number should be clickable. The page should support questions from students, participating companies, and potential sponsors. A contact form can be considered later, but direct contact details are sufficient for the first release and avoid unnecessary storage of enquiry data.

## Questions to Answer Before Development

These questions should be answered before the website architecture and visual design are finalized. Items that are deliberately postponed should be marked as outside the first release rather than left ambiguous.

### Product and Scope

1. What is the final event and website name?
2. What is the single most important action for a student on the website?
3. What is the single most important action for a company?
4. Which features are required for the first tournament, and which belong in later releases?
5. Is the website active year-round or only during a defined registration and recruitment period?
6. Does each yearly tournament have a separate event page and archive?
7. Should the platform support only one tournament at a time?
8. Which information should be publicly visible without an account?
9. Which languages must the first release support: Norwegian, English, or both?
10. What should happen to profiles and accounts between yearly events?

### Brand and Visual Design

1. Does the event already have a logo, color palette, typography, or other brand material?
2. Should the visual identity primarily feel like a golf event, a professional network, or an equal combination?
3. How formal or informal should the tone and interface feel?
4. Which existing websites or brands represent the desired visual direction?
5. Which websites or styles should explicitly be avoided?
6. What photography is available for the course, students, companies, dinner, and afterparty?
7. Who owns the rights to use event, participant, course, and sponsor images?
8. How prominently should sponsors appear without dominating the student experience?
9. Is dark mode required?
10. Are there accessibility requirements beyond the expected WCAG baseline?
11. Should the website be designed mobile-first for use during the event?
12. Which information must be especially quick to find on the event day?

### Navigation and Information Structure

1. What are the primary top-level sections of the website?
2. Should students and companies have separate dashboards after login?
3. Which pages can both user types access?
4. Should event information, company discovery, profiles, and registration be separate workflows?
5. What should the first screen show before registration opens, while registration is open, when the event is full, and after the event?
6. Should users be able to bookmark companies or students?
7. Is direct messaging needed, or should users connect outside the platform?
8. Should notifications appear in the website, by email, by SMS, or through a combination?
9. What information should be searchable globally?
10. Which pages and content must organizers be able to edit without developer assistance?

### Accounts, Roles, and Access

1. Can anyone create a student account, or must students be invited or approved?
2. What proves that a user is an eligible student or recent graduate?
3. Are recent graduates eligible, and if so, for how long after graduation?
4. Who creates the first account for each company?
5. Can a company administrator invite and remove additional company users?
6. Is a company representative always a company user, or can representatives have event-only profiles?
7. Who verifies company accounts, and what evidence is required?
8. Which organizer roles are needed, and what can each role access or change?
9. Can one person have more than one role, such as organizer and company representative?
10. Which profile fields can students hide from companies?
11. Which student fields, if any, can other students see?
12. Can students browse or contact other students?
13. How are suspended, rejected, duplicate, or inactive accounts handled?

### Profiles and Matching

1. Which student profile fields are mandatory before registration can be completed?
2. Is a profile photo mandatory for students and company representatives?
3. Is golf handicap mandatory, optional, or replaceable with “no official handicap”?
4. Which formats and maximum sizes are allowed for CVs and supporting documents?
5. Can students upload more than one CV or language version?
6. Can company users download documents, or only view them in the website?
7. Which filters can companies use when searching for students?
8. Should students be able to indicate interest in specific industries, roles, or companies?
9. Should companies see when a student has viewed or followed their profile?
10. Are the five company qualities used only for communication and filtering, or also for automatic matching?
11. Can companies create any custom quality, or must organizers approve new qualities?
12. How are duplicate or nearly identical qualities prevented?
13. Should students select qualities that describe themselves, and how should those claims be presented?
14. Should users be able to report inaccurate or inappropriate profile content?

### Tournament Registration and Capacity

1. What is the confirmed maximum number of players?
2. How many places are reserved for students and company representatives?
3. How many tournament places are included in each sponsorship package?
4. Can companies buy additional player places beyond their package?
5. Can students register individually only, or can they request teammates?
6. Is registration first-come, application-based, invitation-based, or a combination?
7. When do registration and cancellation close?
8. What happens when the event is full?
9. How does the waiting list work, and how long does a person have to accept an offered place?
10. Which information must be completed before a place is confirmed?
11. Can organizers manually add, remove, or move participants?
12. Can someone attend only the dinner or afterparty?
13. Are guests allowed at the dinner or afterparty?
14. What age restrictions and alcohol rules apply?
15. How are dietary requirements, allergies, accessibility needs, rental clubs, and transport needs collected?
16. Who can see participant lists before and during the event?

### Teams, Handicap, and Scoring

1. Are teams made automatically, manually, or through a combination?
2. What is the desired number of students and company representatives per team?
3. Can participants request or reject specific team placements?
4. Which handicap system and scramble allowance will be used for net scoring?
5. How are players without an official handicap handled?
6. What is the maximum playing handicap allowed in the calculation?
7. When are handicaps locked before the tournament?
8. Who verifies handicaps and approves team changes?
9. Will the website calculate scores, or will Sola GK or external golf software handle scoring?
10. Is live scoring required?
11. Who can enter, edit, approve, and publish scores?
12. How are ties resolved for gross, net, and side competitions?
13. When should team assignments, start holes, and results become visible?

### Payment, Sponsorship, and Refunds

1. What is the final student fee and what does it include?
2. Must students pay immediately to secure a place?
3. Which payment provider and payment methods will be used?
4. Who legally receives student payments and sponsorship payments?
5. Are prices presented including VAT, and what VAT rules apply?
6. Does the organizer need to issue receipts or invoices?
7. Do companies buy sponsorship packages through the website or through manual contracts and invoices?
8. Can discount codes, complimentary places, or organizer-issued invitations be used?
9. What is the cancellation and refund policy?
10. What happens financially if weather or another event forces cancellation or postponement?
11. How are failed, duplicate, disputed, or refunded payments handled?
12. Should payment-provider fees be passed to participants or included in the event budget?

### Event-Day Logistics

1. What practical information must participants receive before arrival?
2. Is digital check-in required, and who operates it?
3. Are QR codes, printed lists, name badges, or all three needed?
4. How are late arrivals and no-shows handled?
5. Where and when do rental-club users collect and pay for equipment?
6. How are last-minute team and handicap changes communicated?
7. Does the organizer need a mobile event-day administration view?
8. Who can access emergency contacts, allergies, and accessibility information?
9. How are schedule changes or urgent notices sent to participants?
10. Should the website show the program, course information, team, starting hole, rules, sponsor stands, dinner seating, and transport details?
11. What must remain available if mobile coverage at the venue is poor?

### Privacy, Consent, and Legal Responsibility

1. Which legal entity owns and operates the website and event?
2. Who is the data controller for student and company information?
3. What legal basis is used for profile processing, event administration, marketing, and recruitment access?
4. What exact consent does a student give when sharing a CV or document?
5. Can consent be given per company, for all verified companies, or both?
6. For how long can companies access student profiles and documents?
7. When are inactive profiles, event data, payment records, and uploaded documents deleted?
8. Can companies download and retain student documents outside the platform, and under which terms?
9. Is sensitive information prohibited in uploaded documents?
10. How can users request access, correction, export, or deletion of their data?
11. Which event communications are required service messages, and which require marketing consent?
12. Is separate consent required for photography and video at the event?
13. How are underage participants handled if they are allowed?
14. What terms must companies accept before accessing student information?
15. Who handles privacy requests, security incidents, and complaints?
16. Which records must be retained for accounting or legal reasons after a user deletes an account?

### Administration and Content Operations

1. Who is responsible for maintaining website content?
2. Which organizer actions require approval from another organizer?
3. Does the admin area need dashboards for capacity, payments, company places, missing information, and document consent?
4. Which data must organizers be able to export, and in which format?
5. Does Sola GK require a specific participant, handicap, team, or dietary export?
6. Should emails and notifications be sent automatically based on registration status?
7. Which reusable email templates are required?
8. Who moderates company profiles, student profiles, images, and custom qualities?
9. Should changes to verified company information require renewed approval?
10. Is an audit history needed for payments, document access, profile approval, and team changes?
11. Who provides user support, and through which channel?
12. What is the process when a participant or company withdraws close to the event?

### Technical Architecture and Integrations

1. Is there an existing hosting provider, domain, email service, or technology preference?
2. Is a custom-built application required, or could parts of registration and payment use existing services?
3. Which external systems must be integrated: payment, email, SMS, accounting, CRM, golf scoring, or Sola GK systems?
4. Does the website need BankID, social login, email login, or another authentication method?
5. Where should private CVs and images be stored?
6. What backup, recovery, and uptime requirements are necessary?
7. What traffic and storage volume should the system support initially and over five years?
8. Which browsers and devices must be supported?
9. Is an API needed for future mobile apps or integrations?
10. Which analytics are allowed, and what should be measured?
11. Which environments are needed for development, testing, and production?
12. Who is responsible for hosting costs, software updates, security patches, and technical support each year?

### Testing and Launch

1. What is the target launch date relative to sponsor sales and student registration?
2. Who has final approval over design, content, privacy, payments, and launch readiness?
3. Which real students, company users, and organizers will test the workflows before launch?
4. What are the acceptance criteria for registration, payment, CV access, and event administration?
5. How will accessibility, mobile layouts, security, and performance be tested?
6. Is a closed pilot needed before public registration opens?
7. How will existing contacts or registrations be imported, if any?
8. What is the fallback process if payment, email, scoring, or check-in fails?
9. Who monitors the website during registration launch and on the event day?
10. What feedback and metrics will determine the priorities for the next yearly event?

## Working Principles

- Make networking useful without turning the experience into a formal job portal.
- Keep student control and transparency central to all document sharing.
- Separate tournament data such as golf handicap from recruitment matching.
- Make company priorities visible and understandable to students.
- Use structured profile data where it improves discovery and administration.
- Start with the smallest feature-complete release that supports the real event workflow.
