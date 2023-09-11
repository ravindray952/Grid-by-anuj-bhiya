# Grid-by-anuj-bhiya                               hdr = header ya jo marzi name likh do
                                                    sbr= side bar  

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>css grid</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="container">
        <div class="box" id="box-1">box-1</div>
        <div class="box" id="box-2">box-2</div>
        <div class="box" id="box-3">box-3</div>
        <div class="box" id="box-4">box-4</div>
        <!-- <div class="box" id="box-5">box-5</div>
        <div class="box" id="box-6">box-6</div>
        <div class="box" id="box-7">box-7</div>
        <div class="box" id="box-8">box-8</div>
        <div class="box" id="box-9">box-9</div>
        <div class="box" id="box-10">box-10</div> -->
    </div>
</body>
</html>


<h1>css part</h1>

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

.container {
    height: 400px;
    border: 2px solid green;
    display: grid;
   row-gap: 20px;
   column-gap:5px;
   /* grid-template-columns: 200px 200px 200px;   20vw 200px 300px or 20% 30% 40% */
   /* grid-template-columns: repeat(auto-fill,100px); */
   /* grid-template-rows: 200px 80px; */
  /* justify-content: center; */
    /* align-content: center; */
    grid-template-areas: "hdr hdr hdr hdr"
                  "sbr  main main main"
                  "sbr  main main main"
                  "ftr ftr ftr ftr";
}




.box {
    border: 2px solid red;
    padding: 12px;
} 

#box-1 {
    grid-area: hdr;
}

#box-2 {
    grid-area: sbr;
}
#box-3 {
    grid-area: main;
}
#box-4 {
    grid-area: ftr;
}
    


#box-5 {
     background-color: rgb(42, 211, 8);
     /* justify-self: end;
     align-self: end; */
     /* grid-column-start: 1;
     grid-column-end: 6; */
  /*  grid-column: 1/-1;   or 1/3  ,1/span 2 yani 2sapna tkjayega     1/-1 (-1 means ulta column third tk) 
    grid-row:  1/3;  or 1/span 4 
    grid-area: 2/12/3/4; */

       
    
}

