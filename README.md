# Policy Jobs Database

Open US jobs in policy research, energy policy and communications at policy institutions, plus data and tech roles at those institutions. Read every day from the employers' own career sites and labelled for visa sponsorship and entry level.

Last updated 2026-10-30 03:33 UTC. Open jobs: 146 (policy research 46, energy policy 68, communications at policy institutions 3, data and tech roles at policy institutions 29).

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
- `applicable`: `yes` for someone with a master's degree and a little work experience: the posting is marked new grad or entry level (title, new-grad lists, or a Claude check of the posting), or it asks for 4 years of experience or less, or it states no number of years. Internships and PhD-only roles are `no`. Blank: not checked yet. `applicable_why` says which of these it was.
- `years_experience`: the years of experience the posting asks for, read by a fixed script; when it gives degree paths ("Bachelor's and 5 years, or Master's and 3") the master's one, and when it lists several requirements the largest. `years_experience_quote` is the sentence. Blank: the posting gives no number.
- `employer_h1b_filings` and `employer_h1b_certified`: H-1B Labor Condition Applications the employer filed and had certified, US Department of Labor data for fiscal year 2025 Q1 to 2026 Q3. `employer_h1b_target_roles` counts the filings for data, software and similar titles, and `employer_h1b_target_entry_level` those at wage levels I–II. A filing is not an approval. Blank: no record matched.
- `posted` is the date the site gives; `first_seen` and `last_seen` are when we saw it.

## Open jobs

### Policy research (46)

| Company | Title | Location | Sponsorship | Applicable | Years | Posted |
|---|---|---|---|---|---|---|
| Charles River Associates | [(2027 Bachelor's/Master's graduates) Economics Consulting Analyst/Associate](https://job-boards.greenhouse.io/charlesriverassociates/jobs/7894191) | Boston, MA, United States; Chicago, IL, United States; New York, NY, United States (+6 more) | sponsors | yes |  | 2026-05-22 |
| The Brattle Group | [Research Analyst (Economics and Finance) - July 2027](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4720811005) | New York, New York, United States; Boston, Massachusetts, United States; Chicago, Illinois, United States (+2 more) | sponsors | yes |  | 2026-08-14 |
| The Brattle Group | [Research Analyst (Economics and Finance) - July 2027](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4732797005) | Chicago, Illinois, United States; Boston, Massachusetts, United States; New York, New York, United States (+2 more) | sponsors | yes |  | 2026-09-10 |
| The Brattle Group | [Research Analyst (Economics and Finance) - July 2027](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4720807005) | Boston, Massachusetts, United States; Chicago, Illinois, United States; New York, New York, United States (+2 more) | sponsors | yes |  | 2026-08-14 |
| The Brattle Group | [Research Analyst (Economics and Finance) - July 2027](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4720810005) | San Francisco, California, United States; Boston, Massachusetts, United States; Chicago, Illinois, United States (+2 more) | sponsors | yes |  | 2026-08-14 |
| The Brattle Group | [Research Analyst (Economics and Finance) - July 2027](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4720808005) | Washington, District of Columbia, United States; Boston, Massachusetts, United States; Chicago, Illinois, United States (+2 more) | sponsors | yes |  | 2026-08-14 |
| The Brattle Group | [Research Analyst (Economics) - July 2027](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4720833005) | Washington, District of Columbia, United States; Boston, Massachusetts, United States; Chicago, Illinois, United States (+1 more) | sponsors | yes |  | 2026-08-14 |
| The Brattle Group | [Research Analyst (Economics) - July 2027](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4720832005) | Chicago, Illinois, United States; Boston, Massachusetts, United States; New York, New York, United States (+1 more) | sponsors | yes |  | 2026-08-14 |
| The Brattle Group | [Research Analyst (Economics) - July 2027](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4720836005) | Boston, Massachusetts, United States; Chicago, Illinois, United States; New York, New York, United States (+1 more) | sponsors | yes |  | 2026-08-14 |
| The Brattle Group | [Research Analyst (Economics) - July 2027](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4720834005) | New York, New York, United States; Boston, Massachusetts, United States; Chicago, Illinois, United States (+1 more) | sponsors | yes |  | 2026-08-14 |
| Center for Global Development | [Fellow/Senior Fellow, Market Shaping Accelerator](https://centerforglobaldevelopment.applytojob.com/apply/jobs/details/nDb6lMwpMb) | Washington, DC | sponsors | no | 5 | 2026-08-07 |
| Center for Global Development | [Policy Fellow - Market Shaping Accelerator](https://centerforglobaldevelopment.applytojob.com/apply/jobs/details/P4s4wWPxHN) | Washington, DC | sponsors | no | 12 | 2026-10-20 |
| Center for Global Development | [Policy Fellow – AI Initiative - DC or London](https://centerforglobaldevelopment.applytojob.com/apply/jobs/details/DLfYmRjhBO) | Washington, DC | sponsors | no | 12 | 2026-10-14 |
| cnas | [Research Assistant/Associate](https://cnas.bamboohr.com/careers/136) | Washington, District of Columbia, United States | unclear | yes | 2 | 2026-07-15 |
| Charles River Associates | [(2028 Bachelor's/Master's graduates) Economics Consulting Analyst/Associate Intern (Summer 2027)](https://job-boards.greenhouse.io/charlesriverassociates/jobs/8120300) | Boston, MA, United States; Chicago, IL, United States; New York, NY, United States (+6 more) | unclear | no |  | 2026-08-28 |
| FAS | [Policy Entrepreneurship, Manager/Senior Manager](https://fas.applytojob.com/apply/jobs/details/Gvh3qKMaXK) | Washington DC, DC | unclear | no | 8 | 2026-10-16 |
| georgetown/wd1/Georgetown_Admin_Careers | [Research Finance & Operations Coordinator - McCourt School of Public Policy - Georgetown University](https://georgetown.wd1.myworkdayjobs.com/Georgetown_Admin_Careers/job/125-E-St-NW-5th-Floor/Research-Finance---Operations-Coordinator---McCourt-School-of-Public-Policy---Georgetown-University_JR27899) | 125 E St NW 5th Floor | unclear | no |  | 2026-10-22 |
| nreca/wd1/External | [Regulatory Affairs Director, Large Loads and Market Policy](https://nreca.wd1.myworkdayjobs.com/External/job/Arlington-VA/Regulatory-Affairs-Director--Large-Loads-and-Market-Policy_R2026-922) | Arlington, VA | unclear | no |  | 2026-09-30 |
| avalerehealth | [Consultant, Policy](https://jobs.lever.co/avalerehealth/4b3acfec-d214-4663-9448-2bcca3108963) | Remote (US); Washington DC | not_mentioned | yes | 4 | 2026-07-24 |
| avalerehealth | [Consultant, Policy (Vaccines)- U.S. Based- REMOTE WORKING OPPORTUNITY](https://jobs.lever.co/avalerehealth/de313ad9-02a4-4c61-941b-3a47665eb715) | Remote (US); Washington DC | not_mentioned | yes | 4 | 2026-07-24 |
| georgetown/wd1/Georgetown_Admin_Careers | [Clinical Research Associate](https://georgetown.wd1.myworkdayjobs.com/Georgetown_Admin_Careers/job/Medical-Center/Clinical-Research-Associate_JR25746-1) | Medical Center | not_mentioned | yes |  | 2026-10-28 |
| Pew Research Center | [Research Assistant, Global Attitudes](https://pewtrusts.wd5.myworkdayjobs.com/CenterExternal/job/Washington-DC-Pew-Research-Center/Research-Assistant--Global-Attitudes_R003309) | Washington, DC (Pew Research Center) | not_mentioned | yes |  | 2026-10-23 |
| Pew Research Center | [Research Associate, U.S. Demography, Race & Ethnicity](https://pewtrusts.wd5.myworkdayjobs.com/CenterExternal/job/Washington-DC-Pew-Research-Center/Research-Associate--US-Demography--Race---Ethnicity_R003304) | Washington, DC (Pew Research Center) | not_mentioned | yes | 3 | 2026-10-07 |
| urban/wd115/Urban-Careers | [Research Assistant – Quantitative (Health, Income, and Benefits Policy Division)](https://urban.wd115.myworkdayjobs.com/Urban-Careers/job/The-Urban-Institute-DC/Research-Assistant---Quantitative--Health--Income--and-Benefits-Policy-Division-_R-801655) | The Urban Institute (DC) | not_mentioned | yes | 1 | 2026-10-23 |
| avalerehealth | [Associate Principal, Policy (Vaccines)- Remote US Work role](https://jobs.lever.co/avalerehealth/412e86d3-8aa9-47c0-8ad9-a5b615990336) | Remote (US); Washington DC | not_mentioned | no | 6 | 2026-09-18 |
| avalerehealth | [Associate Principal, Policy- Drug Pricing (U.S. Based- REMOTE WORK)](https://jobs.lever.co/avalerehealth/5408e673-2063-440e-a204-4d1d05e206b9) | Remote (US); Washington DC | not_mentioned | no | 7 | 2026-09-08 |
| avalerehealth | [Principal, Policy (Medicare Part B) Remote working location](https://jobs.lever.co/avalerehealth/3e1ba274-3939-4d6d-b24a-027f4f49ee05) | Remote (US); Washington DC | not_mentioned | no | 10 | 2026-02-24 |
| fas | [Fisheries Fellow](https://fas.applytojob.com/apply/jobs/details/KRZmXXED18) | United States | not_mentioned | no |  |  |
| FAS | [Senior Advisor, Science Policy – Independent Consultant](https://fas.applytojob.com/apply/jobs/details/Vg5H1WEgkl) | Washington DC, DC | not_mentioned | no | 7 | 2026-10-16 |
| georgetown/wd1/Georgetown_Admin_Careers | [Human Resources Policy & Procedures Specialist](https://georgetown.wd1.myworkdayjobs.com/Georgetown_Admin_Careers/job/2115-Wisconsin-Avenue/Human-Resources-Policy---Procedures-Specialist_JR27579-1) | 2115 Wisconsin Avenue | not_mentioned | no |  |  |
| georgetown/wd1/Georgetown_Admin_Careers | [Policy Director, Economic Dignity Lab - McCourt School of Public Policy - Georgetown University](https://georgetown.wd1.myworkdayjobs.com/Georgetown_Admin_Careers/job/125-E-St-NW-1st-Floor/Policy-Director--Economic-Dignity-Lab---McCourt-School-of-Public-Policy---Georgetown-University_JR27896) | 125 E St NW 1st Floor | not_mentioned | no |  | 2026-10-22 |
| georgetown/wd1/Georgetown_Admin_Careers | [Research Assistant](https://georgetown.wd1.myworkdayjobs.com/Georgetown_Admin_Careers/job/Medical-Center/Research-Assistant_JR27965) | Medical Center | not_mentioned | no |  | 2026-10-30 |
| georgetown/wd1/Georgetown_Admin_Careers | [Senior Research Assistant](https://georgetown.wd1.myworkdayjobs.com/Georgetown_Admin_Careers/job/Medical-Center/Senior-Research-Assistant_JR27811-1) | Medical Center | not_mentioned | no |  | 2026-10-14 |
| rand/wd5/External_Career_Site | [Education Policy Researcher](https://rand.wd5.myworkdayjobs.com/External_Career_Site/job/Santa-Monica-CA-Greater-Los-Angeles-Area/Education-Policy-Researcher_R3667-1) |  | not_mentioned | no |  |  |
| rand/wd5/External_Career_Site | [Health Policy Researcher](https://rand.wd5.myworkdayjobs.com/External_Career_Site/job/Santa-Monica-CA-Greater-Los-Angeles-Area/Health-Policy-Researcher_R3666) |  | not_mentioned | no |  |  |
| The Brattle Group | [Research Analyst Intern (Economics & Finance) - Summer 2027](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4735792005) | Washington, District of Columbia, United States; New York, New York, United States | not_mentioned | no |  | 2026-09-18 |
| The Brattle Group | [Research Analyst Intern (Economics & Finance) - Summer 2027](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4735791005) | New York, New York, United States; Washington, District of Columbia, United States | not_mentioned | no |  | 2026-09-18 |
| The Brattle Group | [Research Analyst Intern (Economics & Finance) - Summer 2027](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4735519005) | San Francisco, California, United States; Washington, District of Columbia, United States | not_mentioned | no |  | 2026-09-18 |
| The Brattle Group | [Research Analyst Intern (Economics & Finance) - Summer 2027](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4735518005) | Washington, District of Columbia, United States; San Francisco, California, United States | not_mentioned | no |  | 2026-09-18 |
| The Brattle Group | [Research Analyst Intern (Economics) - Summer 2027](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4735674005) | Washington, District of Columbia, United States; New York, New York, United States | not_mentioned | no |  | 2026-09-18 |
| The Brattle Group | [Research Analyst Intern (Economics) - Summer 2027](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4735673005) | New York, New York, United States; Washington, District of Columbia, United States | not_mentioned | no |  | 2026-09-18 |
| The Brattle Group | [Research Associate Intern](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4743566005) | San Francisco, California, United States | not_mentioned | no | 3 | 2026-10-14 |
| BRG | [Fall 2027 Economic Consulting Associate](https://thinkbrg.wd5.myworkdayjobs.com/BRG_External_Career_Site/job/Washington-DC/Fall-2027-Economic-Consulting-Associate_JR100972) | Washington, DC; Tampa, FL; New York, NY (+5 more) | no_sponsorship | yes |  | 2026-09-02 |
| BRG | [Policy Analyst – Healthcare Transactions and Strategy](https://thinkbrg.wd5.myworkdayjobs.com/BRG_External_Career_Site/job/Washington-DC/Policy-Analyst---Healthcare-Transactions-and-Strategy_JR101220) | Washington, DC; Remote - USA | no_sponsorship | no | 5 | 2026-10-27 |
| rand/wd5/External_Career_Site | [Information Scientist (Applied Technology Policy)](https://rand.wd5.myworkdayjobs.com/External_Career_Site/job/Washington-DC-DC-Metro-Area/Information-Scientist--Applied-Technology-Policy-_R3628) |  | citizen_or_clearance | no |  |  |
| rand/wd5/External_Career_Site | [RAND Summer Associate Program - POLICY Research](https://rand.wd5.myworkdayjobs.com/External_Career_Site/job/Santa-Monica-CA-Greater-Los-Angeles-Area/RAND-Summer-Associate-Program---POLICY-Research_R3660) |  | citizen_or_clearance | no |  |  |

### Energy policy (68)

| Company | Title | Location | Sponsorship | Applicable | Years | Posted |
|---|---|---|---|---|---|---|
| The Brattle Group | [Energy Analyst (Economics) - July 2027](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4720839005) | Boston, Massachusetts, United States; San Francisco, California, United States; Washington, District of Columbia, United States | sponsors | yes |  | 2026-08-14 |
| The Brattle Group | [Energy Analyst (Economics) - July 2027](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4720840005) | Washington, District of Columbia, United States; Boston, Massachusetts, United States; San Francisco, California, United States | sponsors | yes |  | 2026-08-14 |
| The Brattle Group | [Energy Analyst (Economics) - July 2027](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4735480005) | San Francisco, California, United States; Boston, Massachusetts, United States; Washington, District of Columbia, United States | sponsors | yes |  | 2026-09-18 |
| Charles River Associates | [Associate Principal/Utility Regulation and Finance (Energy practice)](https://job-boards.greenhouse.io/charlesriverassociates/jobs/6283853) | Boston, MA, United States; New York, NY, United States; Washington, DC, United States | sponsors | no | 6 | 2024-09-26 |
| Charles River Associates | [Principal/Utility Regulation and Finance (Energy practice)](https://job-boards.greenhouse.io/charlesriverassociates/jobs/6281772) | Boston, MA, United States; New York, NY, United States; Washington, DC, United States | sponsors | no | 10 | 2024-09-26 |
| Charles River Associates | [Senior Associate/Utility Regulation & Finance (Energy practice)](https://job-boards.greenhouse.io/charlesriverassociates/jobs/5880880) | Boston, MA, United States; New York, NY, United States; Washington, DC, United States | sponsors | no | 5 | 2024-04-04 |
| ProSidian Consulting, LLC | [Energy Analyst (SEED)](https://jobs.smartrecruiters.com/prosidianconsulting/743999950743281) | Salem, OR, United States | unclear | no |  | 2023-12-11 |
| ProSidian Consulting, LLC | [Federal Energy Strategic Support Program Analyst](https://jobs.smartrecruiters.com/prosidianconsulting/743999665668407) | Fort Belvoir, Virginia, United States | unclear | no |  | 2018-02-05 |
| ProSidian Consulting, LLC | [Mid Level Energy Programs Economist](https://jobs.smartrecruiters.com/prosidianconsulting/743999664070643) | Washington, DC, United States | unclear | no |  | 2017-12-22 |
| ProSidian Consulting, LLC | [Senior Level Energy Programs Economist](https://jobs.smartrecruiters.com/prosidianconsulting/743999664070610) | Washington, DC, United States | unclear | no |  | 2017-12-22 |
| ProSidian Consulting, LLC | [Senior Level Energy Programs Regulatory Advisor](https://jobs.smartrecruiters.com/prosidianconsulting/743999664070676) | Washington, DC, United States | unclear | no |  | 2017-12-22 |
| DNV | [Senior Solar Energy Analyst](https://ecyq.fa.em2.oraclecloud.com/hcmUI/CandidateExperience/en/sites/CX_1/job/7831) | Houston, TX, United States; Portland, OR, United States; San Diego, CA, United States (+5 more) | not_mentioned | yes |  | 2026-10-16 |
| DNV | [Senior Wind Energy Analyst](https://ecyq.fa.em2.oraclecloud.com/hcmUI/CandidateExperience/en/sites/CX_1/job/7759) | Seattle, WA, United States; Medford, MA, United States; Portland, OR, United States (+7 more) | not_mentioned | yes |  | 2026-10-21 |
| Dow Jones | [Energy Research Analyst](https://dowjones.wd1.myworkdayjobs.com/Dow_Jones_Career/job/Houston-TX---OPIS/Energy-Research-Analyst_Job_Req_55231) | Houston, TX - OPIS | not_mentioned | yes | 1 | 2026-10-26 |
| Dow Jones | [Senior Research Analyst I - Aromatics & Fibers (Dow Jones Energy)](https://dowjones.wd1.myworkdayjobs.com/Dow_Jones_Career/job/Houston-TX---OPIS/Senior-Research-Analyst-I---Aromatics---Fibers--Dow-Jones-Energy-_Job_Req_55847) | Houston, TX - OPIS | not_mentioned | yes |  | 2026-10-28 |
| Integrated Resources INC | [Energy Analyst](https://jobs.smartrecruiters.com/IntegratedResourcesINC/92068547) | Tampa, FL, United States | not_mentioned | yes |  | 2016-05-09 |
| Trio | [Energy Analyst](https://jobs.lever.co/trio/21f7e6e8-1357-4c31-a04c-36f1e48853a8) | Dublin, Ohio | not_mentioned | yes | 0 | 2026-06-10 |
| Wood Mackenzie | [Research Analyst - Power Market](https://woodmac.wd3.myworkdayjobs.com/woodmaccareers/job/Gurugram-IN/Research-Analyst---Power-Market_JR3402) | Gurugram, IN | not_mentioned | yes | 3 | 2026-10-05 |
| Antora Energy | [Director of Grid Policy](https://job-boards.greenhouse.io/antora/jobs/6128211004) | Remote, USA; Remote - US | not_mentioned | no | 8 | 2026-07-29 |
| Brookhaven Lab | [Research Associate - Electrochemical Energy Storage](https://bnl.wd1.myworkdayjobs.com/externa/job/Upton-NY/Research-Associate---Electrochemical-Energy-Storage_JR102313) | Upton, NY | not_mentioned | no | 5 | 2026-09-29 |
| Central Hudson | [Energy Policy & Regulation Intern](https://cenhud.wd5.myworkdayjobs.com/cenhud/job/Poughkeepsie/Energy-Policy---Regulation-Intern_R2143) | Poughkeepsie | not_mentioned | no |  | 2026-09-11 |
| Citi | [Operational Risk Manager - Platform Utilities and Infrastructure Analyst-VP](https://citi.wd5.myworkdayjobs.com/2/job/Getzville-New-York-United-States/Operational-Risk-Manager---Platform-Utilities-and-Infrastructure-Analyst-VP_26989314) | Getzville New York United States | not_mentioned | no |  | 2026-10-21 |
| Citi | [Operational Risk Manager - Platform Utilities and Infrastructure Analyst-VP](https://citi.wd5.myworkdayjobs.com/2/job/Getzville-New-York-United-States/Operational-Risk-Manager---Platform-Utilities-and-Infrastructure-Analyst-VP_26994689) | Getzville New York United States | not_mentioned | no |  | 2026-10-18 |
| Consolidated Edison | [Energy Storage Contract Planning Analyst](https://ejcu.fa.us6.oraclecloud.com/hcmUI/CandidateExperience/en/sites/CX_1033/job/1000279) | New York, NY, United States | not_mentioned | no |  | 2026-10-21 |
| PJM | [(Sr.) (Lead) (Principal) Energy Analyst/Engineer (II)](https://pjm.wd5.myworkdayjobs.com/pjmcareers/job/Audubon-PA/XMLNAME--Sr---Lead---Principal--Energy-Analyst-Engineer--II-_REQ-2026-4244-1) | Audubon, PA | not_mentioned | no |  |  |
| ProSidian Consulting, LLC | [Mid Level Energy Programs Regulatory Advisor](https://jobs.smartrecruiters.com/prosidianconsulting/743999664070709) | Washington, DC, United States | not_mentioned | no |  | 2017-12-22 |
| SOCOTEC | [Energy Analyst](https://jobs.smartrecruiters.com/Socotec/744000157837276) | Fort Lauderdale, FL, United States | not_mentioned | no |  | 2026-10-26 |
| SOCOTEC | [Energy Analyst](https://jobs.smartrecruiters.com/Socotec/744000157835416) | Boston, MA, United States | not_mentioned | no |  | 2026-10-26 |
| SOCOTEC | [Energy Analyst](https://jobs.smartrecruiters.com/Socotec/744000157836760) | New York, NY, United States | not_mentioned | no |  | 2026-10-26 |
| The Brattle Group | [Energy Analyst Intern (Economics) - Summer 2027](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4735999005) | Boston, Massachusetts, United States | not_mentioned | no |  | 2026-09-18 |
| Veolia Environnement SA | [Energy Market Analyst](https://jobs.smartrecruiters.com/VeoliaEnvironnementSA/744000148315049) | Boston, MA, United States | not_mentioned | no |  | 2026-09-08 |
| Wood Mackenzie | [Senior Research Analyst - Power Market](https://woodmac.wd3.myworkdayjobs.com/woodmaccareers/job/Gurugram-IN/Senior-Research-Analyst---Power-Market_JR2909) | Gurugram, IN | not_mentioned | no |  | 2026-10-14 |
| WSP | [Senior Energy Regulatory Advisor](https://emit.fa.ca3.oraclecloud.com/hcmUI/CandidateExperience/en/sites/CX_2001/job/97265) | United States | not_mentioned | no |  | 2026-10-16 |
| Air Products | [European Energy Analyst](https://airproducts.wd5.myworkdayjobs.com/AP0001/job/Brussels-Belgium/European-Energy-Analyst_JR-2026-21847-1) |  | not checked | no |  | 2026-10-25 |
| Cushman & Wakefield | [Energy Analyst](https://cw.wd1.myworkdayjobs.com/external/job/Chicago-Illinois-USA/Energy-Analyst_R336520) |  | not checked | no |  | 2026-10-01 |
| GE Vernova | [GE Vernova - Energy Technology Analyst Intern - Summer 2027](https://gevernova.wd5.myworkdayjobs.com/only_confidential_executive_recruiting/job/Schenectady/GE-Vernova---Energy-Technology-Analyst-Intern---Summer-2027_R5054316-2) | Schenectady | no_sponsorship | no |  | 2026-10-09 |
| GE Vernova | [Lead Energy Technology Analyst](https://gevernova.wd5.myworkdayjobs.com/only_confidential_executive_recruiting/job/Schenectady/Lead-Energy-Technology-Analyst_R5056535-1) |  | no_sponsorship | no |  | 2026-10-23 |
| ProSidian Consulting, LLC | [Energy Systems Modeler / Energy Market Economic And Regulatory Analysis [DOEOP098103]](https://jobs.smartrecruiters.com/prosidianconsulting/744000028543315) | Washington, DC, United States | no_sponsorship | no |  | 2024-11-26 |
| Booz Allen | [Oil and Gas Energy Analyst](https://bah.wd1.myworkdayjobs.com/bah_jobs/job/Riverdale-MD/Oil-and-Gas-Energy-Analyst_R0248594) | Riverdale, MD | citizen_or_clearance | yes | 3 | 2026-09-02 |
| Booz Allen | [Energy Analyst](https://bah.wd1.myworkdayjobs.com/bah_jobs/job/Riverdale-MD/Energy-Analyst_R0248593) | Riverdale, MD | citizen_or_clearance | no | 7 | 2026-09-02 |
| Booz Allen | [Energy Analyst](https://bah.wd1.myworkdayjobs.com/bah_jobs/job/Riverdale-MD/Energy-Analyst_R0248591) | Riverdale, MD | citizen_or_clearance | no | 7 | 2026-09-02 |
| Booz Allen | [Oil and Gas Energy Analyst](https://bah.wd1.myworkdayjobs.com/bah_jobs/job/Riverdale-MD/Oil-and-Gas-Energy-Analyst_R0248598) | Riverdale, MD | citizen_or_clearance | no | 7 | 2026-09-02 |
| City of Austin | [Energy Market Analyst Senior - Austin Energy](https://austintexas.wd5.myworkdayjobs.com/COA_Careers/job/Austin-Energy-Headquarters/Energy-Market-Analyst-Senior---Austin-Energy_JR105488) | Austin Energy Headquarters | citizen_or_clearance | no |  | 2026-10-17 |
| Mapjects.com | [Energy Strategic Planning/Management Analyst](https://jobs.smartrecruiters.com/Mapjectscom/78342778) | Washington, DC, United States | citizen_or_clearance | no |  | 2014-07-31 |
| Mapjects.com | [Energy Strategic Planning/Management Analyst](https://jobs.smartrecruiters.com/Mapjectscom/78309194) | Fort Belvoir, VA, United States | citizen_or_clearance | no |  | 2014-07-30 |
| Mapjects.com | [PM -  Finance Energy Contract Financial and  Technical Analyst](https://jobs.smartrecruiters.com/Mapjectscom/78427307) | Washington, DC, United States | citizen_or_clearance | no |  | 2014-08-06 |
| National Laboratory of the Rockies | [Integrated Grid Planning and Dynamics - Modeler/Analyst](https://nrel.wd5.myworkdayjobs.com/NLR/job/Golden-CO/Integrated-Grid-Planning-and-Dynamics--Modeler-Analyst_R14343) | Golden, CO | citizen_or_clearance | no | 9 | 2026-06-16 |
| ProSidian Consulting, LLC | [Energy Analyst (Flexible Work Location)](https://jobs.smartrecruiters.com/prosidianconsulting/743999686891909) | Washington, DC, United States | citizen_or_clearance | no |  | 2019-04-17 |
| ProSidian Consulting, LLC | [Energy Budget/Financial Analyst](https://jobs.smartrecruiters.com/prosidianconsulting/743999686844843) | Washington, DC, United States | citizen_or_clearance | no |  | 2019-04-16 |
| ProSidian Consulting, LLC | [Energy Data Management Analyst [PR0003A]](https://jobs.smartrecruiters.com/prosidianconsulting/743999681773781) | Fort Belvoir, VA, United States | citizen_or_clearance | no |  | 2019-01-09 |
| ProSidian Consulting, LLC | [Energy Data Management Senior Analyst [PR0004A]](https://jobs.smartrecruiters.com/prosidianconsulting/743999681773855) | Fort Belvoir, VA, United States | citizen_or_clearance | no |  | 2019-01-09 |
| ProSidian Consulting, LLC | [Energy Infrastructure Risk Analyst](https://jobs.smartrecruiters.com/prosidianconsulting/744000131741149) | Washington, DC, United States; Remote | citizen_or_clearance | no |  | 2026-06-11 |
| ProSidian Consulting, LLC | [Energy Policy Analyst / Energy Market Economic And Regulatory Analysis [DOEOP096101]](https://jobs.smartrecruiters.com/prosidianconsulting/744000028544286) | Washington, DC, United States | citizen_or_clearance | no |  | 2024-11-26 |
| ProSidian Consulting, LLC | [Energy Policy Analyst / Energy Technical Consulting Services [DOEOP003008]](https://jobs.smartrecruiters.com/prosidianconsulting/744000028339276) | Washington, DC, United States | citizen_or_clearance | no |  | 2024-11-25 |
| ProSidian Consulting, LLC | [Energy Policy Analyst / Forecasting And Report Development Support [DOEOP079084]](https://jobs.smartrecruiters.com/prosidianconsulting/744000028669075) | Washington, DC, United States | citizen_or_clearance | no |  | 2024-11-26 |
| ProSidian Consulting, LLC | [Energy Project(s) Manager / Energy Market Economic And Regulatory Analysis [DOEOP097102]](https://jobs.smartrecruiters.com/prosidianconsulting/744000028543581) | Washington, DC, United States | citizen_or_clearance | no |  | 2024-11-26 |
| ProSidian Consulting, LLC | [Energy Systems Analyst / Mapping Support [DOEOP070075]](https://jobs.smartrecruiters.com/prosidianconsulting/744000028750745) | Washington, DC, United States | citizen_or_clearance | no |  | 2024-11-27 |
| ProSidian Consulting, LLC | [Environmental and Technical Research Consultant / Energy Market Economic And Regulatory Analysis [DOEOP099104]](https://jobs.smartrecruiters.com/prosidianconsulting/744000028540180) | Washington, DC, United States | citizen_or_clearance | no |  | 2024-11-26 |
| ProSidian Consulting, LLC | [Geospatial Analyst / Energy Market Economic And Regulatory Analysis [DOEOP100105]](https://jobs.smartrecruiters.com/prosidianconsulting/744000028533210) | Washington, DC, United States | citizen_or_clearance | no |  | 2024-11-26 |
| ProSidian Consulting, LLC | [Legal and Energy Regulatory Expert - Balkans](https://jobs.smartrecruiters.com/prosidianconsulting/743999697464602) | Charlotte, NC, United States | citizen_or_clearance | no |  | 2019-10-16 |
| ProSidian Consulting, LLC | [Market Research Specialist / Energy Market Economic And Regulatory Analysis [DOEOP101106]](https://jobs.smartrecruiters.com/prosidianconsulting/744000028531821) | Washington, DC, United States | citizen_or_clearance | no |  | 2024-11-26 |
| ProSidian Consulting, LLC | [Power Systems Analyst / Modeling Support [DOEOP040045]](https://jobs.smartrecruiters.com/prosidianconsulting/744000028536836) | Washington, DC, United States | citizen_or_clearance | no |  | 2024-11-26 |
| ProSidian Consulting, LLC | [Regulatory Compliance Specialist / Energy Market Economic And Regulatory Analysis [DOEOP102107]](https://jobs.smartrecruiters.com/prosidianconsulting/744000028528555) | Washington, DC, United States | citizen_or_clearance | no |  | 2024-11-26 |
| ProSidian Consulting, LLC | [Senior Energy Policy Analyst (Flexible Work Location)](https://jobs.smartrecruiters.com/prosidianconsulting/743999686894886) | Washington, DC, United States | citizen_or_clearance | no |  | 2019-04-17 |
| ProSidian Consulting, LLC | [Senior Technical Energy Analyst](https://jobs.smartrecruiters.com/prosidianconsulting/743999686895863) | Washington, DC, United States | citizen_or_clearance | no |  | 2019-04-17 |
| ProSidian Consulting, LLC | [Technical Writer and Documentation Specialist / Energy Market Economic And Regulatory Analysis [DOEOP103108]](https://jobs.smartrecruiters.com/prosidianconsulting/744000028526945) | Washington, DC, United States | citizen_or_clearance | no |  | 2024-11-26 |
| ProSidian Consulting, LLC | [Workforce Development Analyst / Energy Market Economic And Regulatory Analysis [DOEOP104109]](https://jobs.smartrecruiters.com/prosidianconsulting/744000028399356) | Washington, DC, United States | citizen_or_clearance | no |  | 2024-11-25 |
| SOSi | [Energy Analyst](https://jobs.smartrecruiters.com/SOSi1/3743990015261556) | Fort Meade, MD, United States | citizen_or_clearance | no |  | 2026-09-15 |

### Communications at policy institutions (3)

| Company | Title | Location | Sponsorship | Applicable | Years | Posted |
|---|---|---|---|---|---|---|
| avalerehealth | [Corporate Marketing Communications Lead](https://jobs.lever.co/avalerehealth/3eb9ca83-01be-4a5f-b27c-9fd932acbeea) | New York, NY; Philadelphia, PA | not_mentioned | yes |  | 2026-08-24 |
| New America | [Senior Communications Associate, Entertainment Initiative](https://newamerica.applytojob.com/apply/jobs/details/zgl7V11NXv) | Washington, DC | not_mentioned | yes | 3 | 2026-10-21 |
| American Institutes for Research | [Communications Specialist, Education Systems & Policy](https://job-boards.greenhouse.io/americaninstitutesforresearch/jobs/5460292008) | US-Remote; Remote (United States) | no_sponsorship | yes | 4 | 2026-10-26 |

### Data and tech roles at policy institutions (29)

| Company | Title | Location | Sponsorship | Applicable | Years | Posted |
|---|---|---|---|---|---|---|
| Charles River Associates | [Associate/Economic Damages and Litigation Support (Risk, Investigations & Analytics practice)](https://job-boards.greenhouse.io/charlesriverassociates/jobs/3090349) | New York, NY, United States | sponsors | yes | 1 | 2021-04-23 |
| Charles River Associates | [Associate/Investigations (Risk, Investigations & Analytics practice)](https://job-boards.greenhouse.io/charlesriverassociates/jobs/1907473) | New York, NY, United States; Washington, DC, United States | sponsors | yes | 3 | 2019-10-08 |
| Charles River Associates | [Senior Platform Engineer (IT Services)](https://job-boards.greenhouse.io/charlesriverassociates/jobs/8263192) | Boston, MA, United States; Chicago, IL, United States; Dallas, Texas, United States | sponsors | yes |  | 2026-10-07 |
| Charles River Associates | [Full Stack Agentic Developer](https://job-boards.greenhouse.io/charlesriverassociates/jobs/7983777) | Boston, MA, United States; Chicago, IL, United States; Dallas, Texas, United States (+4 more) | sponsors | no | 6 | 2026-06-16 |
| Charles River Associates | [Product Manager/Agile Master, AI and Digital Products](https://job-boards.greenhouse.io/charlesriverassociates/jobs/7983867) | Boston, MA, United States; Chicago, IL, United States; Dallas, Texas, United States (+4 more) | sponsors | no | 5 | 2026-06-16 |
| rand/wd5/External_Career_Site | [AI/Bio Research Project Manager, Operations](https://rand.wd5.myworkdayjobs.com/External_Career_Site/job/Washington-DC-DC-Metro-Area/AI-Bio-Research-Project-Manager--Operations_R3657) |  | unclear | no |  |  |
| BRG | [AI Lab Infrastructure Engineer](https://thinkbrg.wd5.myworkdayjobs.com/BRG_External_Career_Site/job/Remote---USA/Ai-Lab-Infrastructure-Engineer_JR100335) | Remote - USA | not_mentioned | yes |  | 2025-11-14 |
| avalerehealth | [Associate Director, Media Data Science](https://jobs.lever.co/avalerehealth/1d1f3668-f195-4074-902a-7623cbf81ea3) | New York, NY; Philadelphia, PA; Washington DC (+1 more) | not_mentioned | no | 6 | 2026-02-26 |
| Code for America | [Lead Product Manager](https://job-boards.greenhouse.io/codeforamerica/jobs/7407338) | Remote (in the U.S.); Varies | not_mentioned | no | 7 | 2025-11-18 |
| Code for America | [Principal Software Engineer](https://job-boards.greenhouse.io/codeforamerica/jobs/8174930) | Remote (in the U.S.); Varies | not_mentioned | no | 10 | 2026-09-11 |
| Code for America | [Staff Data Engineer](https://job-boards.greenhouse.io/codeforamerica/jobs/8188375) | Remote (in the U.S.); Varies | not_mentioned | no | 7 | 2026-09-11 |
| Code for America | [Staff Software Engineer](https://job-boards.greenhouse.io/codeforamerica/jobs/8165204) | Remote (in the U.S.); Varies | not_mentioned | no | 7 | 2026-08-31 |
| American Institutes for Research | [Data Scientist, Project Success and Innovation](https://job-boards.greenhouse.io/americaninstitutesforresearch/jobs/5454172008) | US-Remote; US-VA-Arlington; US-NC-Chapel Hill (+4 more) | no_sponsorship | yes |  | 2026-10-16 |
| American Institutes for Research | [Quantitative Research Associate, Human and Community Development](https://job-boards.greenhouse.io/americaninstitutesforresearch/jobs/5450228008) | US-Remote; US-VA-Arlington; US-NC-Chapel Hill (+4 more) | no_sponsorship | yes | 2 | 2026-10-15 |
| BRG | [Analyst, Data Analytics](https://thinkbrg.wd5.myworkdayjobs.com/BRG_External_Career_Site/job/Washington-DC/Analyst--Data-Analytics_JR101209) | Washington, DC | no_sponsorship | yes | 2 | 2026-10-23 |
| BRG | [Data Analyst - Forensics, Technology, Investigations & Discovery](https://thinkbrg.wd5.myworkdayjobs.com/BRG_External_Career_Site/job/New-York-NY/Data-Analyst---Forensics--Technology--Investigations---Discovery_JR100954) | New York, NY; Chicago, IL; Houston, TX (+1 more) | no_sponsorship | yes | 3 | 2026-10-15 |
| BRG | [Junior Product Manager](https://thinkbrg.wd5.myworkdayjobs.com/BRG_External_Career_Site/job/Remote---USA/Junior-Product-Manager_JR100993) | Remote - USA | no_sponsorship | yes | 1 | 2026-08-27 |
| BRG | [Managing Consultant – Revenue Cycle Analytics – Healthcare](https://thinkbrg.wd5.myworkdayjobs.com/BRG_External_Career_Site/job/Remote---USA/Managing-Consultant---Revenue-Cycle-Analytics---Healthcare_JR101054) | Remote - USA | no_sponsorship | yes |  | 2026-09-01 |
| BRG | [Software Engineer](https://thinkbrg.wd5.myworkdayjobs.com/BRG_External_Career_Site/job/Chicago-IL/Software-Engineer_JR101125) | Chicago, IL; Washington, DC | no_sponsorship | yes | 4 | 2026-10-06 |
| The Brattle Group | [Data and AI Engineer](https://job-boards.greenhouse.io/thebrattlegroup/jobs/4713471005) | Boston, Massachusetts, United States | no_sponsorship | yes | 0 | 2026-07-15 |
| American Institutes for Research | [Senior Quantitative Researcher – CMMI Evaluations](https://job-boards.greenhouse.io/americaninstitutesforresearch/jobs/5448353008) | US-Remote; US-VA-Arlington; US-NC-Chapel Hill (+4 more) | no_sponsorship | no | 7 | 2026-10-08 |
| BRG | [Chicago Office Health Analytics Practice Intern](https://thinkbrg.wd5.myworkdayjobs.com/BRG_External_Career_Site/job/Chicago-IL/Chicago-Office-Health-Analytics-Practice-Intern_JR101039) | Chicago, IL | no_sponsorship | no |  | 2026-08-28 |
| BRG | [Managing Consultant - Healthcare Analytics](https://thinkbrg.wd5.myworkdayjobs.com/BRG_External_Career_Site/job/Washington-DC/Managing-Consultant---Healthcare-Analytics_JR100898) | Washington, DC; Tampa, FL; New York, NY (+4 more) | no_sponsorship | no | 6 | 2026-08-28 |
| BRG | [Managing Consultant - Quality Methodology & Analytics - IHS](https://thinkbrg.wd5.myworkdayjobs.com/BRG_External_Career_Site/job/Baltimore-MD/Managing-Consultant---Quality-Methodology---Analytics---IHS_JR101002) | Baltimore, MD; Washington, DC | no_sponsorship | no | 5 | 2026-08-28 |
| BRG | [Product Manager](https://thinkbrg.wd5.myworkdayjobs.com/BRG_External_Career_Site/job/Remote---USA/Product-Manager_JR101174) | Remote - USA | no_sponsorship | no | 5 | 2026-10-12 |
| BRG | [Software Engineer](https://thinkbrg.wd5.myworkdayjobs.com/BRG_External_Career_Site/job/Washington-DC/Software-Engineer--HAP-Tech_JR100333) | Washington, DC; Remote - USA | no_sponsorship | no | 5 | 2026-02-10 |
| BRG | [Sr. Managing Consultant/Managing Consultant AI Architect - Financial Services Operations & Technology](https://thinkbrg.wd5.myworkdayjobs.com/BRG_External_Career_Site/job/New-York-NY/Sr-Managing-Consultant-Managing-Consultant-AI-Architect---Financial-Services-Operations---Technology_JR101200) |  | no_sponsorship | no |  | 2026-10-24 |
| BRG | [Sr. Managing Consultant/Managing Consultant Data Engineer- Financial Services Operations & Technology](https://thinkbrg.wd5.myworkdayjobs.com/BRG_External_Career_Site/job/New-York-NY/Sr-Managing-Consultant-Managing-Consultant-Data-Engineer--Financial-Services-Operations---Technology_JR101194) |  | no_sponsorship | no |  | 2026-10-24 |
| BRG | [Sr. Managing Consultant/Managing Consultant Full Stack Engineer- Financial Institution Operations & Technology](https://thinkbrg.wd5.myworkdayjobs.com/BRG_External_Career_Site/job/New-York-NY/Sr-Managing-Consultant-Managing-Consultant-Full-Stack-Engineer--Financial-Institution-Operations---Technology_JR101215) |  | no_sponsorship | no |  | 2026-10-27 |

## How it is made

- Jobs come from the employers' public job boards (Greenhouse, Lever, Ashby, Workday and others). Employers whose career sites cannot be read automatically, such as Brookings, NORC and Resources for the Future, are not covered.
- Energy policy jobs are kept at any employer when the title has an energy word (energy, electricity, power markets, utility, grid, renewable, clean energy) together with a policy, regulatory, market, research, economics or analyst word, or says Climate Policy. Investment banking, equity research and accounting roles are left out.
- Policy research and communications jobs are kept only at a fixed list of policy institutions. Senior and management titles are kept too; see `applicable`.
- The labels are a model's reading of short excerpts. Check the posting before you rely on them.
