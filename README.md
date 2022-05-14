# ALTER-TABLE-PRIMARY-KEY-en-Oracle-SQL
#### Como agregar una restriccion primary key luego de haber creado la misma.

```sql
alter table articulos
add constraint codigo_pk
primary key(codigo)
 ```
 ____
 ```sql
 select * from user_cons_columns where constraint_name = 'CODIGO_PK';
 ```
 
 |owner|constraint_name|table_name|column_name|position|
 |:----|:-------------:|---------:|----------:|-------:|
 |CURSO_PLSQL| CODIGO_PK| ARTICULOS| CODIGO|
 
 
```SQL
select * from all_objectS where object_name = 'CODIGO_PK';
```

 |owner|object_name|subobject_name|object_id|object_type|created | last_ddl_time| timestamp|
 |:----|:-------------:|---------:|----------:|----------:|----------:|----------:|-------:|
 |CURSO_PLSQL| CODIGO_PK|null| 20393|20393| index| 14/05/2022| 14/05/2022| 14/05/2022 10:40|

#### CON AMBAS OPCIONES NOS DIRA COMO QUEDO CONFIGURADA NUESTRA LLAVE PRIMARIA
