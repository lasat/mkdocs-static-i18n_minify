# working mkdocs-static-i18n==0.22

`pip install --upgrade -r requirements.txt; mkdocs serve`

1. http://localhost:8000/
  * /css/material.min.css is loaded 
  * /js/material.min.js is loaded 
2. http://localhost:8000/de/
  * /css/material.min.css is loaded 
  * /js/material.min.js is loaded 


# broken with mkdocs-static-i18n>0.22

`pip install --upgrade -r requirements_broken.txt; mkdocs serve`

1. http://localhost:8000/
  * /css/material.min.css is loaded 
  * /js/material.min.js is loaded 
2. http://localhost:8000/de/
  * /css/material.min.css is NOT loaded, instead /css/material.css is requested
  * /js/material.min.js is NOT loaded, instead /js/material.js is requested

