# Identification-of-place-names-from-a-natural-language-sentence

Domain :- AI/ML (Natural Language Processing)

Description:- Building a geospatial querying system based on natural language requires identifying geospatial entities by their names. The scope of this work involves automatically identifying names of places from a sentence. A universe of canonical names (single way of spelling and correct spelling) will be provided in the form of tables. For example, Country, City and State table containing the possible universe of names. It should take into account spelling errors in the names and multiple ways of spelling and mentioning the same entity in the query and map it to canonical name. For example: Given an input: Which of the following saw highest average temperature in January, Maharashtra, Ahmedabad or entire NewZealand? Here, first the system should use
NLP to filter out words that are not names of places, then it must do a fuzzy match to
find candidate canonical names in tables and report the output. Output: Token: Maharashtra,
Canonical name: Maharashtra, table: State Token: Amdabad, Canonical name: Ahmedabad, table: City Token: New-Zealand, Canonical name: newzealand, table: Country Please
note that query need not be a question. It can also be an imperative sentence For example :- Show me a graph of rainfall for Chennai for the month of October
