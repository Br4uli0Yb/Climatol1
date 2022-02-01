Examen final
================
Braulio César Yucra Baquerizo
31/1/2022

## R Markdown

#11. Crear una Función en R para el cálculo del *tc* según la siguiente
fórmula. (1)

``` r
Tiempo_de_concentración <-  function(L, J){
cuerpo <- 0.3*((L/J^(1/4))^0.76)
  return(cuerpo)
}
Tiempo_de_concentración(1200,135)
```

    ## [1] 25.85447

#12.El dataset *airquality* contiene información sobre la velocidad de
viento promedio en Milla/hora, realizar la clasificación de acuerdo a la
Escala Beaufort y Douglas (2)

``` r
#Escala de BEAUFORT
velocidad_de_viento <- 86
if(velocidad_de_viento < 1){
  print("Calma")
}else if(velocidad_de_viento >= 1 & velocidad_de_viento < 3){
  print("Ventolina")
}else if(velocidad_de_viento >= 4 & velocidad_de_viento < 6){
  print("Flojito")
}else if(velocidad_de_viento >= 7 & velocidad_de_viento < 10){
  print("Flojo")
}else if(velocidad_de_viento >= 11 & velocidad_de_viento < 16){
  print("Moderado")
}else if(velocidad_de_viento >= 17 & velocidad_de_viento < 21){
  print("Fresquito")
}else if(velocidad_de_viento >= 22 & velocidad_de_viento < 27){
  print("Fresco")
}else if(velocidad_de_viento >= 28 & velocidad_de_viento < 33){
  print("Frescachón")
}else if(velocidad_de_viento >= 34 & velocidad_de_viento < 40){
  print("Temporal")
}else if(velocidad_de_viento >= 41 & velocidad_de_viento < 47){
  print("Fuerte temporal")
}else if(velocidad_de_viento >= 48 & velocidad_de_viento < 55){
  print("Temporal duro")
}else if(velocidad_de_viento >= 56 & velocidad_de_viento < 63){
  print("Temporal muy duro")
}else{
  print("Temporal huracanado")
}
```

    ## [1] "Temporal huracanado"

``` r
#Escala de Douglas
velocidad_de_viento_2 <- 9
if(velocidad_de_viento_2 < 0){
  print("Llana")
}else if(velocidad_de_viento_2 >= 0 & velocidad_de_viento_2 < 0.25){
  print("Rizada")
}else if(velocidad_de_viento_2 >= 0.25 & velocidad_de_viento_2 < 0.5){
  print("Marejadilla")
}else if(velocidad_de_viento_2 >= 0.5 & velocidad_de_viento_2 < 1.25){
  print("Marejada")
}else if(velocidad_de_viento_2 >= 1.25 & velocidad_de_viento_2 < 2.5){
  print("Fuerte marejada")
}else if(velocidad_de_viento_2 >= 2.5 & velocidad_de_viento_2 < 4){
  print("Gruesa")
}else if(velocidad_de_viento_2 >= 4 & velocidad_de_viento_2 < 6){
  print("Muy gruesa")
}else if(velocidad_de_viento_2 >= 6 & velocidad_de_viento_2 < 9){
  print("Arbolada")
}else if(velocidad_de_viento_2 >= 9 & velocidad_de_viento_2 < 14){
  print("Montañosa")
}else{
  print("Enorme")
}
```

    ## [1] "Montañosa"

This is an R Markdown document. Markdown is a simple formatting syntax
for authoring HTML, PDF, and MS Word documents. For more details on
using R Markdown see <http://rmarkdown.rstudio.com>.

When you click the **Knit** button a document will be generated that
includes both content as well as the output of any embedded R code
chunks within the document. You can embed an R code chunk like this:

``` r
summary(cars)
```

    ##      speed           dist       
    ##  Min.   : 4.0   Min.   :  2.00  
    ##  1st Qu.:12.0   1st Qu.: 26.00  
    ##  Median :15.0   Median : 36.00  
    ##  Mean   :15.4   Mean   : 42.98  
    ##  3rd Qu.:19.0   3rd Qu.: 56.00  
    ##  Max.   :25.0   Max.   :120.00

## Including Plots

You can also embed plots, for example:

![](Examen-final_files/figure-gfm/pressure-1.png)<!-- -->

Note that the `echo = FALSE` parameter was added to the code chunk to
prevent printing of the R code that generated the plot.
