# Policy Jobs Database

Open US jobs in policy research, energy policy and communications at policy institutions, plus data and tech roles at those institutions. Read every day from the employers' own career sites and labelled for visa sponsorship and entry level.

Last updated 2026-10-30 02:33 UTC. Open jobs: 90 (policy research 23, energy policy 48, communications at policy institutions 1, data and tech roles at policy institutions 18).

## Files

- `jobs.csv`: one row per posting, open ones and those closed in the last 30 days. Opens in Excel or Google Sheets.
- `jobs.db`: the same rows as a SQLite database (table `jobs`), for SQL or pandas.

## Columns

- `category`: `policy_research`, `energy_policy`, `policy_communications`, or `data_tech_at_policy_employer`.
- `sponsorship`: what the posting says about visa sponsorship, for someone on F-1 who will need OPT, STEM OPT and then H-1B. Claude (claude-haiku-5-5) labels the sentences that mention visas, sponsorship, citizenship or clearance; `sponsorship_quote` is the sentence it relied on. Values:
  - `sponsors`: says it sponsors, or welcomes F-1/OPT/CPT;
  - `no_sponsorship`: will not sponsor, or does not take F-1/OPT/CPT;
  - `citizen_or_clearance`: needs US citizenship, permanent residency or a security clearance;
  - `unclear`: mentions work authorization but not sponsorship;
  - `not_mentioned`: the posting does not say. This does not mean the employer sponsors; ask the recruiter;
  - blank: not checked yet.
- `entry_level`: `yes` when the title or the posting says new grad, entry level or similar (a Claude check of the posting; PhD-only roles are `no`), `no` otherwise, blank when not checked yet.
- `employer_h1b_filings` and `employer_h1b_certified`: H-1B Labor Condition Applications the employer filed and had certified, US Department of Labor data for fiscal year 2025 Q1 to 2026 Q3. `employer_h1b_target_roles` counts the filings for data, software and similar titles, and `employer_h1b_target_entry_level` those at wage levels I–II. A filing is not an approval. Blank: no record matched.
- `posted` is the date the site gives; `first_seen` and `last_seen` are when we saw it.

## Open jobs

### Policy research (23)

| Company | Title | Location | Sponsorship | Entry level | Posted |
|---|---|---|---|---|---|
| Charles River Associates | [(2027 Bachelor's/Master's graduates) Economics Consulting Analyst/Associate](https://job-boards.greenhouse.io/charlesriverassociates/jobs/7894191) | Boston, MA, United States; Chicago, IL, United States; New York, NY, United States (+6 more) | sponsors | yes | 2026-05-22 |
| The Brattle Group | [Research Analyst (Economics and Finance) - July 2027](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4720811005) | New York, New York, United States; Boston, Massachusetts, United States; Chicago, Illinois, United States (+2 more) | sponsors | yes | 2026-08-14 |
| The Brattle Group | [Research Analyst (Economics and Finance) - July 2027](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4732797005) | Chicago, Illinois, United States; Boston, Massachusetts, United States; New York, New York, United States (+2 more) | sponsors | yes | 2026-09-10 |
| The Brattle Group | [Research Analyst (Economics and Finance) - July 2027](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4720807005) | Boston, Massachusetts, United States; Chicago, Illinois, United States; New York, New York, United States (+2 more) | sponsors | yes | 2026-08-14 |
| The Brattle Group | [Research Analyst (Economics and Finance) - July 2027](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4720810005) | San Francisco, California, United States; Boston, Massachusetts, United States; Chicago, Illinois, United States (+2 more) | sponsors | yes | 2026-08-14 |
| The Brattle Group | [Research Analyst (Economics and Finance) - July 2027](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4720808005) | Washington, District of Columbia, United States; Boston, Massachusetts, United States; Chicago, Illinois, United States (+2 more) | sponsors | yes | 2026-08-14 |
| The Brattle Group | [Research Analyst (Economics) - July 2027](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4720833005) | Washington, District of Columbia, United States; Boston, Massachusetts, United States; Chicago, Illinois, United States (+1 more) | sponsors | yes | 2026-08-14 |
| The Brattle Group | [Research Analyst (Economics) - July 2027](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4720832005) | Chicago, Illinois, United States; Boston, Massachusetts, United States; New York, New York, United States (+1 more) | sponsors | yes | 2026-08-14 |
| The Brattle Group | [Research Analyst (Economics) - July 2027](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4720836005) | Boston, Massachusetts, United States; Chicago, Illinois, United States; New York, New York, United States (+1 more) | sponsors | yes | 2026-08-14 |
| The Brattle Group | [Research Analyst (Economics) - July 2027](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4720834005) | New York, New York, United States; Boston, Massachusetts, United States; Chicago, Illinois, United States (+1 more) | sponsors | yes | 2026-08-14 |
| Charles River Associates | [(2028 Bachelor's/Master's graduates) Economics Consulting Analyst/Associate Intern (Summer 2027)](https://job-boards.greenhouse.io/charlesriverassociates/jobs/8120300) | Boston, MA, United States; Chicago, IL, United States; New York, NY, United States (+6 more) | unclear | no | 2026-08-28 |
| Pew Research Center | [Research Associate, U.S. Demography, Race & Ethnicity](https://pewtrusts.wd5.myworkdayjobs.com/CenterExternal/job/Washington-DC-Pew-Research-Center/Research-Associate--US-Demography--Race---Ethnicity_R003304) | Washington, DC (Pew Research Center) | not_mentioned | yes | 2026-10-07 |
| Pew Research Center | [Research Assistant, Global Attitudes](https://pewtrusts.wd5.myworkdayjobs.com/CenterExternal/job/Washington-DC-Pew-Research-Center/Research-Assistant--Global-Attitudes_R003309) | Washington, DC (Pew Research Center) | not_mentioned | no | 2026-10-23 |
| The Brattle Group | [Research Analyst Intern (Economics & Finance) - Summer 2027](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4735792005) | Washington, District of Columbia, United States; New York, New York, United States | not_mentioned | no | 2026-09-18 |
| The Brattle Group | [Research Analyst Intern (Economics & Finance) - Summer 2027](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4735791005) | New York, New York, United States; Washington, District of Columbia, United States | not_mentioned | no | 2026-09-18 |
| The Brattle Group | [Research Analyst Intern (Economics & Finance) - Summer 2027](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4735519005) | San Francisco, California, United States; Washington, District of Columbia, United States | not_mentioned | no | 2026-09-18 |
| The Brattle Group | [Research Analyst Intern (Economics & Finance) - Summer 2027](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4735518005) | Washington, District of Columbia, United States; San Francisco, California, United States | not_mentioned | no | 2026-09-18 |
| The Brattle Group | [Research Analyst Intern (Economics) - Summer 2027](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4735674005) | Washington, District of Columbia, United States; New York, New York, United States | not_mentioned | no | 2026-09-18 |
| The Brattle Group | [Research Analyst Intern (Economics) - Summer 2027](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4735673005) | New York, New York, United States; Washington, District of Columbia, United States | not_mentioned | no | 2026-09-18 |
| The Brattle Group | [Research Associate Intern](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4743566005) | San Francisco, California, United States | not_mentioned | no | 2026-10-14 |
| urban/wd115/Urban-Careers | [Research Assistant – Quantitative (Health, Income, and Benefits Policy Division)](https://urban.wd115.myworkdayjobs.com/Urban-Careers/job/The-Urban-Institute-DC/Research-Assistant---Quantitative--Health--Income--and-Benefits-Policy-Division-_R-801655) | The Urban Institute (DC) | not_mentioned | no | 2026-10-23 |
| BRG | [Fall 2027 Economic Consulting Associate](https://thinkbrg.wd5.myworkdayjobs.com/BRG_External_Career_Site/job/Washington-DC/Fall-2027-Economic-Consulting-Associate_JR100972) | Washington, DC; Tampa, FL; New York, NY (+5 more) | no_sponsorship | yes | 2026-09-02 |
| BRG | [Policy Analyst – Healthcare Transactions and Strategy](https://thinkbrg.wd5.myworkdayjobs.com/BRG_External_Career_Site/job/Washington-DC/Policy-Analyst---Healthcare-Transactions-and-Strategy_JR101220) | Washington, DC; Remote - USA | no_sponsorship | no | 2026-10-27 |

### Energy policy (48)

| Company | Title | Location | Sponsorship | Entry level | Posted |
|---|---|---|---|---|---|
| The Brattle Group | [Energy Analyst (Economics) - July 2027](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4720839005) | Boston, Massachusetts, United States; San Francisco, California, United States; Washington, District of Columbia, United States | sponsors | yes | 2026-08-14 |
| The Brattle Group | [Energy Analyst (Economics) - July 2027](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4720840005) | Washington, District of Columbia, United States; Boston, Massachusetts, United States; San Francisco, California, United States | sponsors | yes | 2026-08-14 |
| The Brattle Group | [Energy Analyst (Economics) - July 2027](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4735480005) | San Francisco, California, United States; Boston, Massachusetts, United States; Washington, District of Columbia, United States | sponsors | yes | 2026-09-18 |
| Charles River Associates | [Senior Associate/Utility Regulation & Finance (Energy practice)](https://job-boards.greenhouse.io/charlesriverassociates/jobs/5880880) | Boston, MA, United States; New York, NY, United States; Washington, DC, United States | sponsors | no | 2024-04-04 |
| ProSidian Consulting, LLC | [Energy Analyst (SEED)](https://jobs.smartrecruiters.com/prosidianconsulting/743999950743281) | Salem, OR, United States | unclear | no | 2023-12-11 |
| ProSidian Consulting, LLC | [Federal Energy Strategic Support Program Analyst](https://jobs.smartrecruiters.com/prosidianconsulting/743999665668407) | Fort Belvoir, Virginia, United States | unclear | no | 2018-02-05 |
| ProSidian Consulting, LLC | [Mid Level Energy Programs Economist](https://jobs.smartrecruiters.com/prosidianconsulting/743999664070643) | Washington, DC, United States | unclear | no | 2017-12-22 |
| Integrated Resources INC | [Energy Analyst](https://jobs.smartrecruiters.com/IntegratedResourcesINC/92068547) | Tampa, FL, United States | not_mentioned | yes | 2016-05-09 |
| Trio | [Energy Analyst](https://jobs.lever.co/trio/21f7e6e8-1357-4c31-a04c-36f1e48853a8) | Dublin, Ohio | not_mentioned | yes | 2026-06-10 |
| Brookhaven Lab | [Research Associate - Electrochemical Energy Storage](https://bnl.wd1.myworkdayjobs.com/externa/job/Upton-NY/Research-Associate---Electrochemical-Energy-Storage_JR102313) | Upton, NY | not_mentioned | no | 2026-09-29 |
| Central Hudson | [Energy Policy & Regulation Intern](https://cenhud.wd5.myworkdayjobs.com/cenhud/job/Poughkeepsie/Energy-Policy---Regulation-Intern_R2143) | Poughkeepsie | not_mentioned | no | 2026-09-11 |
| Consolidated Edison | [Energy Storage Contract Planning Analyst](https://ejcu.fa.us6.oraclecloud.com/hcmUI/CandidateExperience/en/sites/CX_1033/job/1000279) | New York, NY, United States | not_mentioned | no | 2026-10-21 |
| Dow Jones | [Energy Research Analyst](https://dowjones.wd1.myworkdayjobs.com/Dow_Jones_Career/job/Houston-TX---OPIS/Energy-Research-Analyst_Job_Req_55231) | Houston, TX - OPIS | not_mentioned | no | 2026-10-26 |
| ProSidian Consulting, LLC | [Mid Level Energy Programs Regulatory Advisor](https://jobs.smartrecruiters.com/prosidianconsulting/743999664070709) | Washington, DC, United States | not_mentioned | no | 2017-12-22 |
| SOCOTEC | [Energy Analyst](https://jobs.smartrecruiters.com/Socotec/744000157837276) | Fort Lauderdale, FL, United States | not_mentioned | no | 2026-10-26 |
| SOCOTEC | [Energy Analyst](https://jobs.smartrecruiters.com/Socotec/744000157835416) | Boston, MA, United States | not_mentioned | no | 2026-10-26 |
| SOCOTEC | [Energy Analyst](https://jobs.smartrecruiters.com/Socotec/744000157836760) | New York, NY, United States | not_mentioned | no | 2026-10-26 |
| The Brattle Group | [Energy Analyst Intern (Economics) - Summer 2027](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4735999005) | Boston, Massachusetts, United States | not_mentioned | no | 2026-09-18 |
| Veolia Environnement SA | [Energy Market Analyst](https://jobs.smartrecruiters.com/VeoliaEnvironnementSA/744000148315049) | Boston, MA, United States | not_mentioned | no | 2026-09-08 |
| Wood Mackenzie | [Research Analyst - Power Market](https://woodmac.wd3.myworkdayjobs.com/woodmaccareers/job/Gurugram-IN/Research-Analyst---Power-Market_JR3402) | Gurugram, IN | not_mentioned | no | 2026-10-05 |
| Air Products | [European Energy Analyst](https://airproducts.wd5.myworkdayjobs.com/AP0001/job/Brussels-Belgium/European-Energy-Analyst_JR-2026-21847-1) |  | not checked | no | 2026-10-25 |
| Cushman & Wakefield | [Energy Analyst](https://cw.wd1.myworkdayjobs.com/external/job/Chicago-Illinois-USA/Energy-Analyst_R336520) |  | not checked | no | 2026-10-01 |
| GE Vernova | [GE Vernova - Energy Technology Analyst Intern - Summer 2027](https://gevernova.wd5.myworkdayjobs.com/only_confidential_executive_recruiting/job/Schenectady/GE-Vernova---Energy-Technology-Analyst-Intern---Summer-2027_R5054316-2) | Schenectady | no_sponsorship | no | 2026-10-09 |
| ProSidian Consulting, LLC | [Energy Systems Modeler / Energy Market Economic And Regulatory Analysis [DOEOP098103]](https://jobs.smartrecruiters.com/prosidianconsulting/744000028543315) | Washington, DC, United States | no_sponsorship | no | 2024-11-26 |
| Booz Allen | [Energy Analyst](https://bah.wd1.myworkdayjobs.com/bah_jobs/job/Riverdale-MD/Energy-Analyst_R0248593) | Riverdale, MD | citizen_or_clearance | no | 2026-09-02 |
| Booz Allen | [Energy Analyst](https://bah.wd1.myworkdayjobs.com/bah_jobs/job/Riverdale-MD/Energy-Analyst_R0248591) | Riverdale, MD | citizen_or_clearance | no | 2026-09-02 |
| Booz Allen | [Oil and Gas Energy Analyst](https://bah.wd1.myworkdayjobs.com/bah_jobs/job/Riverdale-MD/Oil-and-Gas-Energy-Analyst_R0248598) | Riverdale, MD | citizen_or_clearance | no | 2026-09-02 |
| Booz Allen | [Oil and Gas Energy Analyst](https://bah.wd1.myworkdayjobs.com/bah_jobs/job/Riverdale-MD/Oil-and-Gas-Energy-Analyst_R0248594) | Riverdale, MD | citizen_or_clearance | no | 2026-09-02 |
| Mapjects.com | [Energy Strategic Planning/Management Analyst](https://jobs.smartrecruiters.com/Mapjectscom/78342778) | Washington, DC, United States | citizen_or_clearance | no | 2014-07-31 |
| Mapjects.com | [Energy Strategic Planning/Management Analyst](https://jobs.smartrecruiters.com/Mapjectscom/78309194) | Fort Belvoir, VA, United States | citizen_or_clearance | no | 2014-07-30 |
| Mapjects.com | [PM -  Finance Energy Contract Financial and  Technical Analyst](https://jobs.smartrecruiters.com/Mapjectscom/78427307) | Washington, DC, United States | citizen_or_clearance | no | 2014-08-06 |
| National Laboratory of the Rockies | [Integrated Grid Planning and Dynamics - Modeler/Analyst](https://nrel.wd5.myworkdayjobs.com/NLR/job/Golden-CO/Integrated-Grid-Planning-and-Dynamics--Modeler-Analyst_R14343) | Golden, CO | citizen_or_clearance | no | 2026-06-16 |
| ProSidian Consulting, LLC | [Energy Analyst (Flexible Work Location)](https://jobs.smartrecruiters.com/prosidianconsulting/743999686891909) | Washington, DC, United States | citizen_or_clearance | no | 2019-04-17 |
| ProSidian Consulting, LLC | [Energy Budget/Financial Analyst](https://jobs.smartrecruiters.com/prosidianconsulting/743999686844843) | Washington, DC, United States | citizen_or_clearance | no | 2019-04-16 |
| ProSidian Consulting, LLC | [Energy Data Management Analyst [PR0003A]](https://jobs.smartrecruiters.com/prosidianconsulting/743999681773781) | Fort Belvoir, VA, United States | citizen_or_clearance | no | 2019-01-09 |
| ProSidian Consulting, LLC | [Energy Infrastructure Risk Analyst](https://jobs.smartrecruiters.com/prosidianconsulting/744000131741149) | Washington, DC, United States; Remote | citizen_or_clearance | no | 2026-06-11 |
| ProSidian Consulting, LLC | [Energy Policy Analyst / Energy Market Economic And Regulatory Analysis [DOEOP096101]](https://jobs.smartrecruiters.com/prosidianconsulting/744000028544286) | Washington, DC, United States | citizen_or_clearance | no | 2024-11-26 |
| ProSidian Consulting, LLC | [Energy Policy Analyst / Energy Technical Consulting Services [DOEOP003008]](https://jobs.smartrecruiters.com/prosidianconsulting/744000028339276) | Washington, DC, United States | citizen_or_clearance | no | 2024-11-25 |
| ProSidian Consulting, LLC | [Energy Policy Analyst / Forecasting And Report Development Support [DOEOP079084]](https://jobs.smartrecruiters.com/prosidianconsulting/744000028669075) | Washington, DC, United States | citizen_or_clearance | no | 2024-11-26 |
| ProSidian Consulting, LLC | [Energy Systems Analyst / Mapping Support [DOEOP070075]](https://jobs.smartrecruiters.com/prosidianconsulting/744000028750745) | Washington, DC, United States | citizen_or_clearance | no | 2024-11-27 |
| ProSidian Consulting, LLC | [Environmental and Technical Research Consultant / Energy Market Economic And Regulatory Analysis [DOEOP099104]](https://jobs.smartrecruiters.com/prosidianconsulting/744000028540180) | Washington, DC, United States | citizen_or_clearance | no | 2024-11-26 |
| ProSidian Consulting, LLC | [Geospatial Analyst / Energy Market Economic And Regulatory Analysis [DOEOP100105]](https://jobs.smartrecruiters.com/prosidianconsulting/744000028533210) | Washington, DC, United States | citizen_or_clearance | no | 2024-11-26 |
| ProSidian Consulting, LLC | [Market Research Specialist / Energy Market Economic And Regulatory Analysis [DOEOP101106]](https://jobs.smartrecruiters.com/prosidianconsulting/744000028531821) | Washington, DC, United States | citizen_or_clearance | no | 2024-11-26 |
| ProSidian Consulting, LLC | [Power Systems Analyst / Modeling Support [DOEOP040045]](https://jobs.smartrecruiters.com/prosidianconsulting/744000028536836) | Washington, DC, United States | citizen_or_clearance | no | 2024-11-26 |
| ProSidian Consulting, LLC | [Regulatory Compliance Specialist / Energy Market Economic And Regulatory Analysis [DOEOP102107]](https://jobs.smartrecruiters.com/prosidianconsulting/744000028528555) | Washington, DC, United States | citizen_or_clearance | no | 2024-11-26 |
| ProSidian Consulting, LLC | [Technical Writer and Documentation Specialist / Energy Market Economic And Regulatory Analysis [DOEOP103108]](https://jobs.smartrecruiters.com/prosidianconsulting/744000028526945) | Washington, DC, United States | citizen_or_clearance | no | 2024-11-26 |
| ProSidian Consulting, LLC | [Workforce Development Analyst / Energy Market Economic And Regulatory Analysis [DOEOP104109]](https://jobs.smartrecruiters.com/prosidianconsulting/744000028399356) | Washington, DC, United States | citizen_or_clearance | no | 2024-11-25 |
| SOSi | [Energy Analyst](https://jobs.smartrecruiters.com/SOSi1/3743990015261556) | Fort Meade, MD, United States | citizen_or_clearance | no | 2026-09-15 |

### Communications at policy institutions (1)

| Company | Title | Location | Sponsorship | Entry level | Posted |
|---|---|---|---|---|---|
| American Institutes for Research | [Communications Specialist, Education Systems & Policy](https://job-boards.greenhouse.io/americaninstitutesforresearch/jobs/5460292008) | US-Remote; Remote (United States) | no_sponsorship | no | 2026-10-26 |

### Data and tech roles at policy institutions (18)

| Company | Title | Location | Sponsorship | Entry level | Posted |
|---|---|---|---|---|---|
| Charles River Associates | [Associate/Economic Damages and Litigation Support (Risk, Investigations & Analytics practice)](https://job-boards.greenhouse.io/charlesriverassociates/jobs/3090349) | New York, NY, United States | sponsors | yes | 2021-04-23 |
| Charles River Associates | [Associate/Investigations (Risk, Investigations & Analytics practice)](https://job-boards.greenhouse.io/charlesriverassociates/jobs/1907473) | New York, NY, United States; Washington, DC, United States | sponsors | yes | 2019-10-08 |
| Charles River Associates | [Full Stack Agentic Developer](https://job-boards.greenhouse.io/charlesriverassociates/jobs/7983777) | Boston, MA, United States; Chicago, IL, United States; Dallas, Texas, United States (+4 more) | sponsors | no | 2026-06-16 |
| Charles River Associates | [Product Manager/Agile Master, AI and Digital Products](https://job-boards.greenhouse.io/charlesriverassociates/jobs/7983867) | Boston, MA, United States; Chicago, IL, United States; Dallas, Texas, United States (+4 more) | sponsors | no | 2026-06-16 |
| BRG | [AI Lab Infrastructure Engineer](https://thinkbrg.wd5.myworkdayjobs.com/BRG_External_Career_Site/job/Remote---USA/Ai-Lab-Infrastructure-Engineer_JR100335) | Remote - USA | not_mentioned | no | 2025-11-14 |
| American Institutes for Research | [Data Scientist, Project Success and Innovation](https://job-boards.greenhouse.io/americaninstitutesforresearch/jobs/5454172008) | US-Remote; US-VA-Arlington; US-NC-Chapel Hill (+4 more) | no_sponsorship | yes | 2026-10-16 |
| American Institutes for Research | [Quantitative Research Associate, Human and Community Development](https://job-boards.greenhouse.io/americaninstitutesforresearch/jobs/5450228008) | US-Remote; US-VA-Arlington; US-NC-Chapel Hill (+4 more) | no_sponsorship | yes | 2026-10-15 |
| BRG | [Junior Product Manager](https://thinkbrg.wd5.myworkdayjobs.com/BRG_External_Career_Site/job/Remote---USA/Junior-Product-Manager_JR100993) | Remote - USA | no_sponsorship | yes | 2026-08-27 |
| The Brattle Group | [Data and AI Engineer](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4713471005) | Boston, Massachusetts, United States | no_sponsorship | yes | 2026-07-15 |
| BRG | [Analyst, Data Analytics](https://thinkbrg.wd5.myworkdayjobs.com/BRG_External_Career_Site/job/Washington-DC/Analyst--Data-Analytics_JR101209) | Washington, DC | no_sponsorship | no | 2026-10-23 |
| BRG | [Chicago Office Health Analytics Practice Intern](https://thinkbrg.wd5.myworkdayjobs.com/BRG_External_Career_Site/job/Chicago-IL/Chicago-Office-Health-Analytics-Practice-Intern_JR101039) | Chicago, IL | no_sponsorship | no | 2026-08-28 |
| BRG | [Data Analyst - Forensics, Technology, Investigations & Discovery](https://thinkbrg.wd5.myworkdayjobs.com/BRG_External_Career_Site/job/New-York-NY/Data-Analyst---Forensics--Technology--Investigations---Discovery_JR100954) | New York, NY; Chicago, IL; Houston, TX (+1 more) | no_sponsorship | no | 2026-10-15 |
| BRG | [Managing Consultant - Healthcare Analytics](https://thinkbrg.wd5.myworkdayjobs.com/BRG_External_Career_Site/job/Washington-DC/Managing-Consultant---Healthcare-Analytics_JR100898) | Washington, DC; Tampa, FL; New York, NY (+4 more) | no_sponsorship | no | 2026-08-28 |
| BRG | [Managing Consultant - Quality Methodology & Analytics - IHS](https://thinkbrg.wd5.myworkdayjobs.com/BRG_External_Career_Site/job/Baltimore-MD/Managing-Consultant---Quality-Methodology---Analytics---IHS_JR101002) | Baltimore, MD; Washington, DC | no_sponsorship | no | 2026-08-28 |
| BRG | [Managing Consultant – Revenue Cycle Analytics – Healthcare](https://thinkbrg.wd5.myworkdayjobs.com/BRG_External_Career_Site/job/Remote---USA/Managing-Consultant---Revenue-Cycle-Analytics---Healthcare_JR101054) | Remote - USA | no_sponsorship | no | 2026-09-01 |
| BRG | [Product Manager](https://thinkbrg.wd5.myworkdayjobs.com/BRG_External_Career_Site/job/Remote---USA/Product-Manager_JR101174) | Remote - USA | no_sponsorship | no | 2026-10-12 |
| BRG | [Software Engineer](https://thinkbrg.wd5.myworkdayjobs.com/BRG_External_Career_Site/job/Chicago-IL/Software-Engineer_JR101125) | Chicago, IL; Washington, DC | no_sponsorship | no | 2026-10-06 |
| BRG | [Software Engineer](https://thinkbrg.wd5.myworkdayjobs.com/BRG_External_Career_Site/job/Washington-DC/Software-Engineer--HAP-Tech_JR100333) | Washington, DC; Remote - USA | no_sponsorship | no | 2026-02-10 |

## How it is made

- Jobs come from the employers' public job boards (Greenhouse, Lever, Ashby, Workday and others). Employers whose career sites cannot be read automatically, such as Brookings, NORC and Resources for the Future, are not covered.
- Energy policy jobs are kept at any employer when the title has an energy word (energy, electricity, power markets, utility, grid, renewable, clean energy) together with a policy, regulatory, market, research, economics or analyst word, or says Climate Policy. Investment banking, equity research and accounting roles are left out.
- Policy research and communications jobs are kept only at a fixed list of policy institutions; senior and management titles are left out everywhere.
- The labels are a model's reading of short excerpts. Check the posting before you rely on them.
