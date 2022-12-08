[How to generate scaffold with Infyom Laravel Generator](https://www.youtube.com/watch?v=g6Rp98_0inQ&list=PL0wCC44AhrC3JHzcB5qmjYkm70OaoKegg&index=4&t=81s)

selectTable:users:name,id

php artisan infyom:scaffold User --fromTable --tableName=users --ignoreFields=email_verified_at,remember_token



otras opciones
:api \$MODEL_NAME$ --paginate=10  
:scaffold \$MODEL_NAME --datatables=true  
:scaffold \$MODEL_NAME --views=index,create,edit,show  
:scaffold \$MODEL_NAME --factory  
:scaffold \$MODEL_NAME --seeder    
:scaffold \$MODEL_NAME --fieldsFile=filename_from_model_schema_directory_OR_path_from_base_directory_OR_absolute_file_path
:scaffold \$MODEL_NAME --tableName=custom_table_name  
:scaffold \$MODEL_NAME --fromTable --tableName=$TABLE_NAME
:scaffold \$MODEL_NAME --fromTable --tableName=$TABLE_NAME --connection=connectionName  
:api_scaffold Post --skip=routes,migration,model  
:scaffold \$MODEL_NAME --primary=custom_name_id
:scaffold \$MODEL_NAME --plural=AuthorBooks
:scaffold \$MODEL_NAME --prefix=admin
:scaffold \$MODEL_NAME --ignoreFields=geo_location,last_login
:scaffold \$MODEL_NAME --forceMigrate
:api \$MODEL_NAME --resources=true

| upported HTML Input Types & Formats                            | Valid Examples                     |
| -------------------------------------------------------------- | ---------------------------------- |
| text                                                           | text                               |
| textarea                                                       | textarea                           |
| email                                                          | email                              |
| date                                                           | date                               |
| number                                                         | number                             |
| password                                                       | password                           |
| file (partially supported)                                     | file                               |
| select                                                         |                                    |
| select,value1,value2,value3                                    | select,Daily,Weekly,Monthly        |
| select,label1:value1,label2:value2,label3:value3               | select,Sunday:0,Monday:1,Tuesday:2 |
| select from existing table                                     |                                    |
| selectTable:tableName:column1,column2                          | selectTable:users:name,id          |
| Note:where column1 is Option Label and column2 is Option Value | selectTable:categories:title,id    |
| checkbox                                                       | checkbox                           |
| checkbox,value                                                 | checkbox,yes                       |
|                                                                | checkbox,1                         |
| radio                                                          |                                    |
| radio,label1,label2                                            | radio,Male,Female                  |
| radio,label1:value1,label2:value2                              | radio,Yes:1,No:0                   |
| toggle switch                                                  | toggle-switch                      |