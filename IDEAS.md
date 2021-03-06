
# Ideas, Suggestions

###  field ids

Each field has its own ID. ID gets included in the JSON output. Benefits: 

- the Factbook contains descriptions for all fields which could be referenced/downloaded/extracted using this ID. 

- The field description could also be used to create a mapping "field_names_used_in_JSON" 
  to their respective original text (or: as an alternative, the original field name 
  could be included in the output itself)

- the Factbook contains text tables containing the raw data for numeric fields, 
  so there is no need to sanitize the fields to get their numeric values.  
  To reference these raw data tables the field ID is needed
  the Factbook contains field listings (the compiled values of fields for all countries). 
  To reference these tables the field ID is needed, again


### pseudo header section

Include a pseudo section in the JSON output
to make the entries more descriptive / self-contained (to be located at the top, before intro):

~~~
"header" : {
   "country" : "Austria",
   "fips" : "at"
}
~~~

The header, if included, should contain

- name of the territory in question, e.g. Virgin Islands
- name of parent region, e.g. Central America and Caribbean
- dependency, e.g (territory of the US)
- date of last update, e.g Page last updated on June 20, 2014
- fips code, e.g., VQ
- date & time when the json file was produced


### Thanks

Eckhard Licher
