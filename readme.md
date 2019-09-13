INSTRUCCIONES:

1) haz un ng g pipe filter
2) pega el contenido de filterPipe.ts en el mismo archivo (o sustituye)
3) ve al html en cuestión donde quieras usar el pipe de filtrado
4) haz un input de search y pones en el [(ngModel)]="foodSearch"
5) En donde este la lista a filtrar, en el div o lo que sea añade el pipe:

 <div class="food-card" *ngFor = "let food of foods | filter:'name':foodSearch; let i = index">

6) en el ts del componente añade el campo:
 - foodSearch: string = "";

 LISTO, ya tienes tu pipe de filtrado
