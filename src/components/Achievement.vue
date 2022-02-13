<template>
  <div>
    <modal 
    name="example"
    shiftX= '0.98'
    shiftY = '0.02'
    width = "20%"
    height = "10%"
    >
    <img :src="lien[this.num]"/>
    <!--{{texte[this.num]}} -->
    </modal>
  </div>
</template>

<script>
export default {
  data() {
    return {
      "texte": [
          "A small step for monke a giant step for man",
          "GORILLAAAAS",
          "Warning it's hot",
          "It's Britney bitch",
          "Maybe you can trade emeralds there",
          "",
          "The first fan fiction",
          "Animal abuse begins",
          "",
          "Steam powered",
          "The beggining of the end",
          "50k"
      ],
      "lien": [
          "https://images-ext-1.discordapp.net/external/46qR7tefwRu_jxqcKAdirWDzmW8xERqPuNXg0uFOJQ0/https/www.abc.net.au/reslib/200905/r374157_1738132.jpg",
          "https://upload.wikimedia.org/wikipedia/commons/b/bb/Gorille_des_plaines_de_l%27ouest_%C3%A0_l%27Espace_Zoologique.jpg",
          "https://cdn.radiofrance.fr/s3/cruiser-production/2018/05/a1872be9-22d4-4ac6-82d0-e314fae8ecd0/838_feu.jpg",
          "https://images.immediate.co.uk/production/volatile/sites/4/2019/10/GettyImages-183882286-528c62a.jpg?quality=90&resize=460,306",
          "https://upload.wikimedia.org/wikipedia/commons/8/8a/Biface_%28trihedral%29_Amar_Merdeg%2C_Mehran%2C_Ilam%2C_Lower_Paleolithic%2C_National_Museum_of_Iran.jpg",
          "https://i.imgur.com/Gtcovsd.jpg",
          "https://upload.wikimedia.org/wikipedia/commons/b/b8/Ggantija_Temples%2C_Xaghra%2C_Gozo.jpg",
          "https://ichef.bbci.co.uk/news/1024/media/images/63514000/jpg/_63514348_protoelamite464.jpg",
          "https://upload.wikimedia.org/wikipedia/commons/thumb/f/f8/Detail_of_Les_tres_riches_heures_-_March.jpg/220px-Detail_of_Les_tres_riches_heures_-_March.jpg",
          "https://multimediaman.files.wordpress.com/2012/09/papyrus.jpg",
          "https://upload.wikimedia.org/wikipedia/commons/thumb/3/30/Standard_Oil.jpg/330px-Standard_Oil.jpg",
          "https://s3.amazonaws.com/appforest_uf/f1605786836050x199045280153180350/epitech-logo-signature-noir.png"
      ]
    }
  },
  props: {
      num: Number
  },
  name: 'MyComponent',
  mounted () {
      this.$modal.show('example')
  }
}
</script>


