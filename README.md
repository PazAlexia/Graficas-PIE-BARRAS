# Graficas-PIE-BARRAS
#grafica pie
pie(frec)
#labels le ponemos la etiqueta debe de ser vector
pie(frec,labels=c("IMSS","ISSSTE","Otra","No recibe","No especificado"))
#main para poner el titulo
pie(frec,labels=c("IMSS","ISSSTE","Otra","No recibe","No especificado"),
    main = "Institución de atención medica")
pie(frec,labels=c("IMSS","ISSSTE","Otra","No recibe","No especificado"),
    main = "Institución de atención medica")
#col para poner color a cada sector en este caso es un vector
pie(frec,labels=c("IMSS","ISSSTE","Otra","No recibe","No especificado"),
    main="Institución de atención medica",col = c("green","red","blue","gray","yellow"))
    
#grafica de barras
#sacamos las frecuencias de las variables a utilizar
frec1<-table(sd1$EDA5C)
View(frec1)
#ponemos titulo
barplot(frec1,main="cinco grupos de edad")
#col funciona silimar al pie
barplot(frec1,main="cinco grupos de edad", col = c("green","red","blue","gray","yellow"))
#etiquetas se pueden poner con names.arg
barplot(frec1,main="grafica 1.cinco grupos de edad", col = c("green","red","blue","gray","yellow"),
        names.arg = c("menor","14 a 24","25 a 44","45 a 64","65 y mas","n.e"))
#ylim 
frec1
barplot(frec1,main="grafica 1.cinco grupos de edad", col = c("green","red","blue","gray","yellow"),
        names.arg = c("menor","14 a 24","25 a 44","45 a 64","65 y mas","n.e"),ylim = c(0,85000))
#tambien podemos poner los nombres en nuestra variable con names
names(frec1)<-c("menor","14 a 24","25 a 44","45 a 64","65 y mas","n.e")
#xlab, ylab para colocar el nombre a los ejes
barplot(frec1,main="grafica 1.cinco grupos de edad", col = c("green","red","blue","gray","yellow"),
        names.arg = c("menor","14 a 24","25 a 44","45 a 64","65 y mas","n.e"),xlab="Edad",
        ylab="POblacion",ylim = c(0,85000))
