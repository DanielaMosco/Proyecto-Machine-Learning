# Proyecto-Machine-Learning-Clustering
Este repositorio contiene el proyecto final del curso de Machine Learning en Azure ML Studio para obtener el diploma en Análisis de Datos.

## Muestra del código
```Azure Machine Learning Studio
select *,
       case when Attrition_Flag = 'Existing Customer' then 1 else 0 end as AF_Existing,
       case when Attrition_Flag = 'Attrited Customer' then 1 else 0 end as AF_Attrited,
       case when Education_Level = 'Graduate' or 'High School' or 'Unknown' or 'Uneducated' then 1 else 0 end as EL_Graduate_HighSchool_Unk_Uned,
       case when Gender = 'M' then 1 else 0 end as G_Male,
       case when Gender = 'F' then 1 else 0 end as G_Female,
       case when Marital_Status = 'Married' or 'Single 'then 1 else 0 end as MS_Married_Single,
       case when Income_Category = 'Less than $40K' then 1 else 0 end as IC_less40,
       case when Card_Category = 'Blue' then 1 else 0 end as CC_Blue
from t1;
```

## Muestra del resultado

<img align="left" alt="png" src="https://user-images.githubusercontent.com/98499583/151684104-df758c06-0fd8-40df-8c31-dca2c2e4f5b9.png" width="40%" height="auto" />
