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

Direct messaging, a custom-built scoring system, and year-round job listings can be considered after the core workflow is proven. Automated scramble-team proposals are required in the first release.

## Confirmed Participation and Payment Model

1. **Student eligibility:** Active students and people who graduated within the previous two years can participate. A connection to Stavanger is not required.
2. **Admission:** Participation should combine invitations with online registration. An eligible student with a complete profile, mandatory CV, available student capacity, and successfully completed payment should receive immediate confirmation without manual organizer approval. The organizer can still manually manage invitations, capacity, duplicates, and exceptional cases.
3. **Capacity allocation:** The working capacity is 72 players: approximately 54 student places and 18 company-representative places. Final capacity and reserved numbers remain configurable per event.
4. **Payments:** Students should pay their participation fee directly through the website. Companies should receive sponsorship-package invoices outside the website rather than completing a consumer checkout.
5. **Team allocation:** The platform should automatically propose balanced scramble teams using handicap, the desired student/company distribution, and anonymous company favorites. The organizer must review and approve teams before they are published.
6. **Recent graduates:** A participant is considered a recent graduate for up to two years after completing their education.
7. **Eligibility verification:** Formal proof of active-student or recent-graduate status is not required. Applicants should declare their current study or graduation details, and the organizer retains the ability to review suspicious or inaccurate registrations.
8. **Company access period:** Verified companies can access participating student profiles and shared CVs until one week after the tournament ends. Access must then be revoked automatically. Authorized company users may view and download shared CVs during this period. Because downloaded copies cannot technically be revoked, companies must accept purpose limitation, retention, deletion, and non-sharing terms before access; downloads should be logged and clearly attributed where practical.
9. **Refund policy:** Cancellation, no-show, postponement, weather, and refund rules will be decided later and must be published before payments open.
10. **Sponsorship places:** Sponsorship packages should include a fixed standard number of player places. Organizers must be able to override the number for an individually negotiated package without changing the published standard package.
11. **Team composition:** Team size should remain flexible until actual registration numbers are known. Allocation should use three- or four-player teams as required while targeting approximately 25% company representatives and 75% students across the field. A four-player team would normally contain one company representative and three students, but exact composition is not guaranteed.
12. **Players without an official handicap:** They may participate and should use handicap 54 for team allocation and scoring calculations, subject to final confirmation of the competition rules with Sola GK.
13. **Waiting list:** Once the 54 student places are filled, otherwise eligible students should automatically join a waiting list without paying. Payment is requested only when a place is offered and accepted.
14. **Included attendance:** A confirmed player place includes the golf tournament, dinner, and afterparty as one package. Players do not select or purchase these components separately, although attendance and dietary details may still be collected for planning.
15. **Minimum age:** All participants must be at least 18 years old on the event date because the package includes the afterparty and may involve alcohol service.
16. **Team publication:** Approved scramble teams and starting holes should be published a few days before the tournament. The exact publication deadline remains to be set in the event schedule.
17. **Allocation priority:** The team algorithm must prioritize balanced total team handicap before applying anonymous company favorites. Favorites are a secondary preference and must not materially undermine sporting balance.
18. **Student fee:** The final fee will be determined later from the approved event budget. It must be configurable per yearly event rather than hard-coded in the website.
19. **Student package:** The student fee includes green fee, food, dinner, afterparty, and any transport the organizer chooses to include in the event package. Golf-club or other equipment rental is excluded and handled separately.
20. **Transport:** Participants are expected to arrange their own transport to and from Sola GK. No shared transport is currently included in the event package.
21. **Rental clubs:** Students can indicate that they need rental clubs during registration. The organizer should include this need in the Sola GK export, while availability, collection, and payment are handled directly by Sola GK.
22. **Dietary information:** Every participant must answer the dietary-requirements and allergy questions, including explicitly selecting "none" when they have no requirements. Access must be restricted to organizers and relevant food-service personnel.
23. **Check-in:** A participant list in the admin area is sufficient. The organizer will manually mark arrivals; participant-facing QR codes or self-service digital check-in are not required.

The company-favorite limit, waiting-list offer deadline, post-event retention of privately stored CVs, authority for final scramble and handicap rules, and exact urgent-notification channels are intentionally deferred decisions. They must be settled before the related workflows are implemented or registration opens.

### Sponsorship Capacity and Course Activities

- The event should accept as many suitable sponsors as practical rather than setting a fixed sponsor count.
- Sponsors from the same industry may participate at the same time; no sponsorship package provides automatic industry exclusivity.
- Sponsorship does not automatically include a player place; places are controlled by the selected package or individual agreement and the overall 18-place company allocation.
- All approved sponsors receive the same standard level of digital logo visibility on the homepage sponsor strip and sponsor page. Package price should not automatically change logo size or prominence.
- Physical sponsor stands and course activities remain limited by venue capacity, pace of play, safety, and Sola GK approval.
- A sponsor may request a stand, branded activity, or competition at a specific hole when included in its agreement.
- Specific-hole allocation must be approved and managed by the organizer in coordination with Sola GK; sponsors cannot claim a hole directly through self-service booking.
- Sponsorship packages and prices should not be published as self-service products on the website. Interested companies should use the partnership call to action and contact the organizer for an individual offer.
- A company profile and its users may be prepared in advance, but sponsor access to student profiles and CVs must remain disabled until the organizer records the sponsorship agreement as paid.

### Recommended Student Payment Approach

Vipps MobilePay ePayment is the preferred option for student payments, subject to commercial onboarding and confirmation of the legal payment recipient. It supports initiating a payment, redirecting the user to complete it, retrieving status, capturing the payment, and issuing full or partial refunds.

The integration must:

- Create payments server-side with unique, idempotent references.
- Keep API credentials out of the browser and source control.
- Verify payment state through the API and authenticated webhooks rather than trusting the browser redirect.
- Confirm a tournament place only according to the agreed admission and payment rules.
- Handle abandoned, failed, duplicate, expired, cancelled, and refunded payments.
- Store the payment reference and necessary accounting status without storing payment-card details.
- Automatically send the student a payment and place-confirmation email after verified successful payment.
- Be tested against the Vipps MobilePay test environment before production use.

Sponsor contracts, invoices, payment follow-up, and receipts should be handled manually by the organizer outside the website. The admin dashboard only needs a controlled status for recording agreement and payment state and enabling access.

Official implementation guidance: [Vipps MobilePay ePayment API quick start](https://developer.vippsmobilepay.com/docs/APIs/epayment-api/quick-start/).

### Recommended Legal Structure

The preferred direction, pending final confirmation by the organizer, is to establish a non-profit association as the event organizer, provided the event continues to operate without a profit motive. A Norwegian association is an organization created by its members around an agreed purpose. It should be formed with a founding meeting and document, bylaws, a board, and clear signing authority, then registered in the Norwegian Register of Legal Entities to obtain an organization number.

This would give the recurring event a separate organizational identity and a clearer basis for a bank account, venue and sponsor agreements, company invoicing, Vipps MobilePay onboarding, bookkeeping, and responsibility for personal data. Payments and contracts should not be handled privately by the organizer once the association is operational.

Association status does not automatically make every activity tax-free or exempt it from VAT, accounting, or reporting obligations. The actual purpose, income, sponsorship arrangements, and recurring economic activity must be assessed before sales and sponsorship packages open. Official starting points: [Brønnøysund Registers: registering an association](https://www.brreg.no/lag-og-foreninger/registrere-lag-eller-forening/) and [Norwegian Tax Administration: tax-exempt organizations](https://www.skatteetaten.no/bedrift-og-organisasjon/rapportering-og-bransjer/bransjer-med-egne-regler/frivillige-og-ideelle-organisasjoner/skattefrie-organisasjoner/).

### Tournament Scoring System

Sola GK's existing tournament system should be the source of truth for scoring and results. GolfBox is the likely system and is designed for tournament administration, including entries, start lists, real-time scoring, standings, result lists, and winner lists. This must be confirmed directly with Sola GK.

The website should initially integrate results at one of these levels:

1. **Reliable baseline:** Link directly from the event-day dashboard to the specific GolfBox live-scoring and results page.
2. **Preferred presentation:** Embed the official public GolfBox live-scoring page if GolfBox and Sola GK permit framing and it works securely and responsively.
3. **Deeper integration:** Import or synchronize structured tournament data only if GolfBox provides an approved API, export, or partner integration for this use.

No undocumented scraping or duplicate scoring system should be used. The website can retain an approved final result export for the yearly archive. The supported integration method, result URL, data ownership, and organizer permissions must be confirmed with Sola GK before development.

### Event-Day Presentation

- Participant name badges are not required.
- Dinner seating is unassigned; participants choose their own seats.
- The organizer can build and publish a structured event program in the admin area. Each item should support a time, title, location, short description, ordering, and current status or update.
- The result experience should expose both gross and net team standings from GolfBox when the available GolfBox result view or approved integration supports them.
- Winners of closest to the pin, longest drive, and straightest drive should be published on the event result page and retained in the yearly archive.
- The organizer must be able to enter or correct side-competition winners manually if GolfBox does not supply those results.

## Confirmed Account Administration

- The first release requires exactly one organizer administrator account and an admin dashboard. Additional organizer roles and admin invitations are not required.
- The organizer will create and manage company access rather than delegating user invitations to a company administrator.
- Company users must not be able to create, invite, remove, or approve other company users.
- Each authorized company employee must have a personal login. Shared company credentials are not permitted.
- Every organizer-approved personal user belonging to a participating sponsor may search student profiles and view or download shared CVs during the defined access period. Access is not limited to sponsors with player places.
- Every such user must individually accept the company-access and document-use terms before access is enabled.
- The organizer admin must be able to create, activate, suspend, edit, and remove company users and associate them with the correct company profile.
- Administrative actions affecting access to student profiles, CVs, payments, or team allocation should be logged.
- Company users can edit their own company profile and opportunity links through a simple, guided interface. Company administration must not expose unrelated technical or event-management settings.
- Jobs, internships, and graduate opportunities should primarily be represented by a short title, opportunity type, optional summary, and external link to the company's official listing rather than recreating a complete applicant-tracking system.
- Approved company users may publish company-profile changes and opportunity links directly without per-change organizer approval. The organizer must still be able to review, unpublish, edit, or remove inappropriate or outdated content and suspend publishing access.
- Confirmed students may continue editing their profile and replacing their CV through the tournament period. Relevant changes should be reflected immediately for authorized company users and recorded where appropriate.

### Authentication

- Students, company users, and the organizer administrator sign in with an email address and password.
- Email ownership must be verified before an account becomes active.
- Secure password reset, rate limiting, session expiration, and protection against credential stuffing are required.
- Passwords must be processed by the authentication provider using an appropriate one-way password hash and must never be stored or logged in plain text.
- Multi-factor authentication is not required for students, company users, or the single administrator in the first release. It should remain available as a later security improvement, especially for administrator and CV-access roles.

### Student Account and Registration Flow

The registration flow should create a pending student account before payment so the required profile and CV can be securely associated with the correct person:

1. The student enters an email address, which becomes the username, and creates a password.
2. The student verifies the email address.
3. The student provides a telephone number and completes all mandatory profile, eligibility, event, dietary, consent, and CV fields.
4. The system checks age, profile completeness, student capacity, and waiting-list state.
5. When capacity is available, the student completes Vipps payment.
6. A verified successful payment activates the confirmed participant status immediately and triggers the confirmation email.

If student capacity is already full, the completed account joins the unpaid waiting list and does not proceed to payment. The organizer can retrieve the registered student's email address and telephone number through the access-controlled admin view and appropriate exports. Company accounts are created manually by the organizer.

### Required Admin Exports

The admin dashboard must export operational data in Excel and/or CSV format for Sola GK and event operations. Export options must cover:

- Participant identity and contact information required for administration.
- Student and company allocation.
- Golf handicap and no-official-handicap status.
- Approved teams and starting holes.
- Dietary requirements and allergies in a separately access-controlled export.
- Rental-club requirements.
- Attendance and manual check-in status.
- Payment and sponsorship status where required for internal reconciliation.

Exports must include only the fields needed for their stated recipient and purpose. CVs, transcripts, company favorites, and recruitment notes must never appear in general Sola GK or event-operation exports.

### Editable Content

The admin dashboard should function as a constrained content-management interface. The organizer can edit changing operational content without developer assistance, including:

- Event date, venue, registration period, capacity, price, and event status.
- Homepage announcements, countdown target, and calls to action.
- Tournament information, practical details, program, and event-day contact information.
- Sponsors, logos, links, and sponsor-strip order.
- Contact-page details.
- Standard notification and email-template content.
- Historical event summary, approved results links, and approved gallery content.

The organizer should edit structured fields and predefined sections, not arbitrary page layouts, navigation architecture, security rules, or visual-system code.

### Email Templates

The admin area must provide reusable Norwegian and English templates for registration and payment confirmation, waiting-list status and place offers, incomplete-profile reminders, payment reminders where applicable, team and starting-hole publication, practical pre-event information, urgent changes, and post-event follow-up. Automated sends must record delivery status and avoid duplicate messages.

### Hosting and Backups

- Application data, private CVs, profile images, and backups must be hosted with appropriate providers in the EU/EEA.
- Private documents must use access-controlled object storage and must not be exposed through permanent public URLs.
- Automated encrypted backups, restoration procedures, retention periods, and periodic restore testing are required.
- Hosting, storage, authentication, email, analytics, and backup vendors must be documented and covered by appropriate data-processing terms before production launch.

### Analytics

Use limited, privacy-conscious analytics to measure public website visits, registration-funnel completion, confirmed registrations, and aggregate views of company profiles and opportunity links. Do not expose individual student browsing behavior to companies, and do not use CV access logs for marketing analytics. Prefer an EU/EEA-hosted, cookieless configuration where practical; any non-essential tracking must follow the required consent rules.

### Event Email Domain

After the event name and domain are selected, automated messages and public contact should preferably use an event-domain address such as `kontakt@[event-domain]`. The domain must be configured with SPF, DKIM, and DMARC for reliable delivery. The organizer's Gmail address remains the temporary public contact until the event-domain mailbox is ready.

## Required First Release

The first tournament release must include the complete core platform rather than postponing major workflows. It requires:

1. Student registration, personal accounts, mandatory profiles, CV upload, and Vipps payment.
2. Company profiles and organizer-managed personal accounts for company employees.
3. Student discovery of participating companies and their prioritized qualities.
4. Company search and filtering of participating students, including authorized CV viewing and download for all approved sponsor users.
5. Private student bookmarks and anonymous company favorites.
6. Automated scramble-team proposals using handicap, participant ratios, and company favorite weighting, followed by organizer approval.
7. Capacity management, immediate confirmation, and an unpaid student waiting list.
8. Organizer administration for users, content, payments, capacity, profiles, access, exports, and team management.
9. Tournament, program, sponsor, contact, profile, event-day, and historical archive pages.
10. GolfBox result linking or an approved embedded result view.
11. Norwegian and English interface support.
12. Company publication of specific job openings, internships, graduate roles, and other relevant opportunities during the active event period.

### Mandatory Student Profile

Before a student can pay and receive a confirmed place, the profile must contain:

- Full name.
- Profile photo.
- University or educational institution and study location.
- Field of study and current year of study, or graduation details for recent graduates.
- Place of origin.
- Areas of interest.
- Relevant skills and experience.
- Official golf handicap or the no-official-handicap selection, which uses 54.
- CV upload.
- Required privacy, event, and document-sharing acknowledgements.

## Confirmed Product Decisions

1. **Working name:** Use `[Event Name]` as a placeholder. The final name will be selected later.
2. **Primary student action:** Create a student profile, explore participating companies, and understand what each company does and looks for in students.
3. **Primary company action:** Browse participating students and privately favorite interesting candidates. Favorites anonymously increase the chance of sharing a scramble team.
4. **First-release scope:** The complete core platform defined in Required First Release must be available for the first tournament.
5. **Active period:** The website only needs to be operational before and during the tournament. Exact opening and closing dates remain to be decided.
6. **Yearly events and archive:** Each tournament should have its own event page. Information from previous tournaments should be retained in a historical archive and database where legally permitted.
7. **Active tournaments:** The platform only needs to support one active tournament at a time for now.
8. **Public information:** Visitors without an account should be able to see general event information, the schedule, participating companies, sponsors, and appropriate historical event information. Student profiles, private participant details, favorites, CVs, and supporting documents must never be public.
9. **Languages:** Users should be able to switch between Norwegian and English using a standard language selector. User-provided profile content does not need automatic translation in the first release.
10. **Accounts between events:** Student profiles and accounts should be retained for possible reuse in later tournaments. Returning students must review and confirm their information before registering for a new event. Company accounts and editable company profiles are recreated for each yearly event.

Historical participant data must not automatically become a public participant directory. Retention of personal profiles, CVs, documents, and company access must be covered by clear consent, retention periods, deletion rights, and applicable data-protection requirements. Public historical pages should use an explicitly approved subset of event information.

## Confirmed Privacy and Participant Visibility

1. **Sponsor consent:** A student gives one explicit consent covering profile and CV access by all verified sponsor companies, rather than selecting companies individually. The consent screen must identify the eligible recipient group, purpose, access period, download possibility, and consequences of withdrawal before the student confirms.
2. **Downloaded CV retention:** The platform revokes sponsor access one week after the tournament, but a company may retain a CV it downloaded for a legitimate, stated recruitment process. The student must be informed that downloaded copies cannot be remotely deleted. The receiving company becomes responsible for its copy and must handle retention, security, purpose limitation, data-subject requests, and deletion under its own privacy obligations and the accepted sponsor terms. Unlimited or unrelated reuse is not permitted; an exact default retention expectation remains to be defined.
3. **Student participant directory:** Signed-in participating students may see a limited directory of other participants. It may show name, profile photo, field and year of study, institution or study location, place of origin, and areas of interest. It must not expose CVs, transcripts, supporting documents, contact details, company favorites, private notes, payment information, or other restricted fields.
4. **Photography:** Registration must include a separate, clearly presented photography and publication choice. The implementation and event process must record the choice and allow the organizer to identify participants who have not agreed before publishing identifiable images.
5. **Self-service deletion:** Students must be able to request or initiate deletion of their account, profile, photo, and uploaded documents. The system may retain only records that must be kept for accounting, legal claims, fraud prevention, or other documented obligations, and these retained records must no longer remain available as an active profile.

Fields such as study program, interests, and place of origin are still personal data when connected to an identifiable participant, even though they are less sensitive than a CV or transcript. They must therefore remain behind participant login and be covered by the privacy notice.

## Confirmed Discovery Timing

1. Students with a pending account may browse participating company profiles before paying or receiving a confirmed place.
2. Specific job and internship links and the ability to favorite companies are available only after the student's payment and participation are confirmed.
3. A paid and verified sponsor's authorized users can see a student's shared profile and CV as soon as that student's payment and participation are confirmed; access does not wait for registration to close.
4. Company user accounts and editable company profiles are event-specific and should not remain active for reuse the following year. The organizer creates new company accounts and obtains updated profile information for each event. An approved, limited public record of previous participating companies may still remain in the historical event archive.
5. A dedicated global emergency switch for all company access is not required in the first admin interface. The organizer must still be able to suspend individual company users and companies, and ordinary incident-response controls must remain available at the system or authentication-provider level.

## Confirmed Contact and Matching Rules

1. Verified sponsor users with active access may see the confirmed student's email address and telephone number in addition to the shared profile and CV. Students must be informed of this disclosure before confirming participation.
2. Signed-in students may see the attending company representatives' approved professional contact information and LinkedIn links. Representatives must control and confirm which details are published.
3. Company search should remain simple because the initial participant pool is limited. Useful filters include field of study, year of study or graduation year, institution or study location, areas of interest, relevant skills or experience, and place of origin. The interface should not present a large or overly complex filter system for 54 students.
4. Students are not required to select five personal qualities. The five-quality structure applies only to what companies say they prioritize.
5. Student views, bookmarks, and favorites of company profiles are private. Companies must not be shown which individual students viewed or favorited them, and this behavior must not be used as a hidden recruitment score.

## Confirmed Document and Opportunity Rules

1. Student CVs must be uploaded as PDF files.
2. A transcript is optional and must be stored and protected under the same rules as the CV.
3. The student profile may include one optional **Other document** upload for a relevant certificate, reference, application letter, or similar supporting material. It should also use PDF unless a later requirement justifies another format.
4. Companies may create their own five prioritized core qualities rather than being limited to organizer-approved suggestions. The interface can still suggest existing qualities and normalize obvious duplicates for consistent display and filtering.
5. Job and internship links do not expire or become hidden automatically at the event date or listed application deadline. Company users and the organizer can remove or unpublish outdated links manually. The interface should still support an optional application deadline and clearly display when that date has passed.

File-size limits, malware scanning, replacement behavior, and final retention periods must be defined during technical design. Private documents must never be attached directly to notification emails.

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
