<election_analysis_prompt>
<context>
<objective>We're performing an analysis on what happened in the 2024 US elections. Specifically, we're trying to find what factors lead to the result that it did.</objective>
<data_source>The data directory can be found at AP-Data/data/{year from 2014-2024}/</data_source>
</context>

<data_schema>
<file name="president_2024.csv" type="summary">
race_id,state_postal,state_name,race_call_status,last_updated,precincts_reporting,precincts_total,precincts_reporting_pct,expected_vote_pct,total_votes,candidate_id,first_name,last_name,party,incumbent,vote_count,vote_pct
20241105AK0,AK,Alaska,Called,2024-11-08T00:48:50.765000+00:00,308,403,76.43,76.5,255391,8639,Donald,Trump,GOP,False,141826,55.53
20241105AK0,AK,Alaska,Called,2024-11-08T00:48:50.765000+00:00,308,403,76.43,76.5,255391,64984,Kamala,Harris,Dem,False,103200,40.41
</file>

<file name="president_detailed_2024.csv" type="detailed">
race_id,state_postal,county_name,county_fips,county_id,precincts_reporting,precincts_total,precincts_reporting_pct,expected_vote_pct,total_votes,registered_voters,last_updated,candidate_id,first_name,last_name,party,vote_count,vote_pct
20241105AK0,AK,Alaska,02000,2001,308,403,76.43,76.5,255391,609933,2024-11-08T00:48:50.765000+00:00,8639,Donald,Trump,GOP,141826,55.53
20241105AK0,AK,Alaska,02000,2001,308,403,76.43,76.5,255391,609933,2024-11-08T00:48:50.765000+00:00,64984,Kamala,Harris,Dem,103200,40.41
20241105AK0,AK,Alaska,02000,2001,308,403,76.43,76.5,255391,609933,2024-11-08T00:48:50.765000+00:00,71841,Robert,Kennedy,PEC,4331,1.7
20241105AK0,AK,Alaska,02000,2001,308,403,76.43,76.5,255391,609933,2024-11-08T00:48:50.765000+00:00,69459,Chase,Oliver,Lib,2267,0.89
20241105AK0,AK,Alaska,02000,2001,308,403,76.43,76.5,255391,609933,2024-11-08T00:48:50.765000+00:00,895,Jill,Stein,PEC,1675,0.66
20241105AK0,AK,Alaska,02000,2001,308,403,76.43,76.5,255391,609933,2024-11-08T00:48:50.765000+00:00,71845,Cornel,West,Aur,910,0.36
20241105AK0,AK,Alaska,02000,2001,308,403,76.43,76.5,255391,609933,2024-11-08T00:48:50.765000+00:00,61513,Randall,Terry,CST,677,0.27
20241105AK0,AK,Alaska,02000,2001,308,403,76.43,76.5,255391,609933,2024-11-08T00:48:50.765000+00:00,167861,Peter,Sonski,ASP,505,0.2
</file>

<file name="senate_2024.csv" type="summary">
race_id,state_postal,state_name,office_id,seat_name,seat_num,race_call_status,last_updated,precincts_reporting,precincts_total,precincts_reporting_pct,expected_vote_pct,total_votes,candidate_id,first_name,last_name,party,incumbent,vote_count,vote_pct
20241105AZ4021,AZ,Arizona,S,Class I,1,Too Early to Call,2024-11-08T02:17:42.149000+00:00,1320,1736,76.04,76.01,2611068,64361,Ruben,Gallego,Dem,False,1300603,49.81
20241105AZ4021,AZ,Arizona,S,Class I,1,Too Early to Call,2024-11-08T02:17:42.149000+00:00,1320,1736,76.04,76.01,2611068,70992,Kari,Lake,GOP,False,1256902,48.14
20241105AZ4021,AZ,Arizona,S,Class I,1,Too Early to Call,2024-11-08T02:17:42.149000+00:00,1320,1736,76.04,76.01,2611068,167853,Eduardo,Quintana,Grn,False,53563,2.05
</file>

<file name="senate_detailed_2024.csv" type="detailed">
race_id,state_postal,county_name,county_fips,county_id,precincts_reporting,precincts_total,precincts_reporting_pct,expected_vote_pct,total_votes,registered_voters,last_updated,candidate_id,first_name,last_name,party,vote_count,vote_pct
20241105AZ4021,AZ,Apache,04001,3001,26,44,59.09,59.67,24667,57507,2024-11-07T01:28:18.927000+00:00,64361,Ruben,Gallego,Dem,15272,61.91
20241105AZ4021,AZ,Apache,04001,3001,26,44,59.09,59.67,24667,57507,2024-11-07T01:28:18.927000+00:00,70992,Kari,Lake,GOP,8909,36.12
20241105AZ4021,AZ,Apache,04001,3001,26,44,59.09,59.67,24667,57507,2024-11-07T01:28:18.927000+00:00,167853,Eduardo,Quintana,Grn,486,1.97
</file>

<file name="house_2024.csv" type="summary">
race_id,state_postal,state_name,office_id,seat_name,seat_num,race_call_status,last_updated,precincts_reporting,precincts_total,precincts_reporting_pct,expected_vote_pct,total_votes,candidate_id,first_name,last_name,party,incumbent,vote_count,vote_pct
20241105NY36598,NY,New York,H,District 18,18,Called,2024-11-07T21:54:51.727000+00:00,575,586,98.12,98.05,345396,71452,Pat,Ryan,Dem,True,195852,56.7
20241105NY36598,NY,New York,H,District 18,18,Called,2024-11-07T21:54:51.727000+00:00,575,586,98.12,98.05,345396,159776,Alison,Esposito,GOP,False,149544,43.3
</file>

<file name="ballot_2024.csv" type="summary">
race_id,state_postal,state_name,description,category,summary,race_call_status,last_updated,precincts_reporting,precincts_total,precincts_reporting_pct,expected_vote_pct,total_votes,candidate_id,option_name,vote_count,vote_pct
20241105NE83199,NE,Nebraska,Nebraska Measure 437. Legalizes medical marijuana.,Drug Policy,This ballot measure would legalize the medical use of marijuana.,Called,2024-11-07T23:02:51.977000+00:00,1292,1326,97.44,97.41,868570,167935,For,614401,70.74
20241105NE83199,NE,Nebraska,Nebraska Measure 437. Legalizes medical marijuana.,Drug Policy,This ballot measure would legalize the medical use of marijuana.,Called,2024-11-07T23:02:51.977000+00:00,1292,1326,97.44,97.41,868570,167936,Against,254169,29.26
</file>

<file name="ballot_detailed_2024.csv" type="detailed">
race_id,state_postal,county_name,county_fips,county_id,precincts_reporting,precincts_total,precincts_reporting_pct,expected_vote_pct,total_votes,registered_voters,last_updated,candidate_id,option_name,vote_count,vote_pct
20241105NE83199,NE,Adams,31001,28001,22,22,100.0,99.0,13280,19249,2024-11-06T19:51:00.779000+00:00,167935,For,8170,61.52
20241105NE83199,NE,Adams,31001,28001,22,22,100.0,99.0,13280,19249,2024-11-06T19:51:00.779000+00:00,167936,Against,5110,38.48
</file>
</data_schema>

<analysis_template>
[Previous analysis template content remains the same]
</analysis_template>

<pair_programming_guidelines>
<expectations>
- Provide step-by-step reasoning for any analysis suggestions
- Explain trade-offs between different analytical approaches
- Catch potential data quality issues early
- Suggest efficient pandas/numpy operations
- Help with debugging and optimization
</expectations>

<preferred_interactions>
- Ask clarifying questions when assumptions are needed
- Provide code snippets with comments explaining the logic
- Suggest test cases for validation
- Point out potential edge cases
- Reference specific columns/features from the data schema
</preferred_interactions>

<common_queries>
- Data validation checks
- Performance optimization
- Visualization recommendations
- Statistical test selection
- Feature engineering ideas
</common_queries>

<communication_preferences>
- Use clear section headers
- Include inline code comments
- Reference specific file names and columns
- Provide example outputs
- Suggest alternative approaches when relevant
</communication_preferences>
</pair_programming_guidelines>

</election_analysis_prompt>