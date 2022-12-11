# Data Modeling | Designing Tables

*Database design for a pet adoption agency that rescues animals and seeks to find them owners who are a good match for them.*

### animals
- animal_id **SERIAL PRIMARY KEY**
- species_id **FOREIGN KEY**
- animal_name
        
### species
- species_id **SERIAL PRIMARY KEY**
- species_name
 
### prospects
- prospect_id **SERIAL PRIMARY KEY**
- name
- phone_number
- email

##### Middle Table
*This table pairs prospective owners with their preferred species to help match prospects with potential animals to adopt.*

species_prospects
- animal_prospect_id **SERIAL PRIMARY KEY**
- prospect_id **FOREIGN KEY**
- species_id **FOREIGN KEY**


## Design Visual Map
![Flow chart of db mapping](./DB-Design%402x.png)