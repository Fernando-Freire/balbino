<template>
   <div class="album py-5 bg-light">
    <div class="container">
      <div class="row">
        <Card :coffeeData='{
                          id: 1,
                          name: "Tradicional",
                          image: "https://http2.mlstatic.com/D_NQ_NP_684659-MLB40292588889_122019-O.webp",
                          weight: "500g",
                          characteristics: ["Bebida Dura", "Torrado e Moído","Torra Média"],
                          link: "https://produto.mercadolivre.com.br/MLB-1661998143-cafe-balbino-tradicional-500-g-_JM"
                        }'
         />
        <Card :coffeeData='{
                            id: 2,
                            name: "Gourmet",
                            image: "https://http2.mlstatic.com/D_NQ_NP_2X_930880-MLB40293464375_122019-F.webp",
                            weight: "1kg",
                            characteristics: ["Estritamente mole","Café em grãos","Torra clara"],
                            link: "https://produto.mercadolivre.com.br/MLB-1661998153-cafe-balbino-gourmet-em-gros-1-kg--_JM"
                          }' />
        <Card :coffeeData='{
                            id: 3,
                            name: "Premium",
                            image: "https://http2.mlstatic.com/D_NQ_NP_717779-MLB40293298718_122019-O.webp",
                            weight: "500g",
                            characteristics: ["Estritamente Mole","Torrado e Moído","Torra Clara"],
                            link: "https://produto.mercadolivre.com.br/MLB-1662000830-cafe-balbino-premium-500-gramas-_JM"
                          }' />
      </div>
    </div>
  </div>
</template>

