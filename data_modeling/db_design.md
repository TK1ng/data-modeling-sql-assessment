# Data Modeling | Designing Tables

*Database design for a pet adoption agency that rescues animals and seeks to find them owners who are a good match for them.*

### animals
- animal_id <span style="color: #687dd4;">**SERIAL PRIMARY KEY**</span>
- species_id <span style="color: #ff7978;">**FOREIGN KEY**</span>
- animal_name
        
### species
- species_id <span style="color: #687dd4;">**SERIAL PRIMARY KEY**</span>
- species_name
 
### prospects
- prospect_id <span style="color: #687dd4;">**SERIAL PRIMARY KEY**</span>
- name
- phone_number
- email

##### Middle Table
*This table pairs prospective owners with their preferred species to help match prospects with potential animals to adopt.*

species_prospects
- animal_prospect_id <span style="color: #687dd4;">**SERIAL PRIMARY KEY**</span>
- prospect_id <span style="color: #ff7978;">**FOREIGN KEY**</span>
- species_id <span style="color: #ff7978;">**FOREIGN KEY**</span>


## Design Visual Map
![Flow chart of db mapping](./DB-Design%402x.png)