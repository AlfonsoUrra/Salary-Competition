![image](https://github.com/AlfonsoUrra/Salary-Competition/blob/main/img/money-gf460fcd18_1920.jpg)

# Salary-Competition
 
 
 
## Descripción del proyecto
EL proyecto trata de hacer un modelo predictivo en un dataset de Salaries, entrenar diferentes modelos y buscar el más óptimo y que mejor explique la variable salary.
 
 
 
# Organización de los datos
 
 
## Outliers
  
 Realizo un estudio de los outliers para entender un poco mejor el dataset. También analizo los máximos y mínimos. Relizo la media de los salarios y a través delos Quartiles establezco unos límites para los valores.
 
![image](https://github.com/AlfonsoUrra/Salary-Competition/blob/main/img/Quartiles%20outliers.png)
![image](https://github.com/AlfonsoUrra/Salary-Competition/blob/main/img/Outliers.png)

## Eliminación columnas
Después de explorar los datos y no encontrar ningún nulo ni valor duplicado, entendemos que hay ciertos dartos que no aportan valor al modelo como las columnas "Salary" y "Salary Currency".Estas columnas se encuentran recogidas en "Salary_in_usd". Por lo que decidí eliminarlas.

![image](https://github.com/AlfonsoUrra/Salary-Competition/blob/main/img/data%201%20and%20data%202.png)
 
 
 #3 Transformación Datos
  
En la columna "job_title" consideré que era conveniente agruparla en menos valores únicos para poder manejar los datos de forma más eficaz. Por lo que condensé todos los trabajos en 4 variables.
 
- "ml" o "machine learning", que sea "ml"
- "anayst" que sea "analyst"
-  engineer que sea "engineer"
- scientist que sea "scientist"
- otros que sean "other"
 
 
 
En la columna experience decidí agrupar por salarios. Realicé una medie por categoría de experiencia con sus salarios y establecí límites para poner las etiquetas correspondientes a cada nivel de experiencia.
 
 ![image](https://github.com/AlfonsoUrra/Salary-Competition/blob/main/img/experience%20and%20salary.png)
 
 
 El resto de datos los convertí de categóricos a numéricos con get dummies.
 
 # Elección modelo
 
 Después de realizar un lazyRegressor y estudiar diferentes modelos me quedo con el modelo MLP Regressor.  Entreno los datos y testeo en el nuevo dataset.
![image](https://github.com/AlfonsoUrra/Salary-Competition/blob/main/img/Modelos%20.png)
 
# Conclusión
 
 
El Machine Learning y la estadística ofrecen un agran cantidad de posibilidades a la hora de entender y analzar los datos. Son herramientas poderosas y complejas que castigan el desconocimiento y el manejo pobre de los datos. La mayor parte del éxito reside en entender y limpiar los datos de forma correcta, entender el problema y aplicar el modelo que mejor se ajuste. Ante la falta de conocimientos o la poca familiaridad con esta tecnología, la experienca me ha guiado a optar por el camino conocido que mejor domine, aunque parezca sencillo es efixaz y funciona
 
