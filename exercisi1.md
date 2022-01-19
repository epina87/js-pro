```js
[ // 100 usuaris
    {
        id: 0,
        nivell: 100, // numero del 0-100
        animals: [ // una llista d'animal preferits (de 4 a 8)
        'elefant',
        'pantera',
        'tigre',
        'foca',
    ]},
    {
        id:  ,
        nivell: 50, // numero del 0-100
        animals: [ // una llista d'animal preferits (de 4 a 8)
        'dofi',
        'gos',
        'zebra',
        'foca',
    ]},
]
```

1. fas una llista de 20 animals
   ```js
    llistaAnimals = ['llop','serp','tigre','coala','oreneta','gat','gos','girafa','elefan','rinoceront','cocodril','ximpanze','izart','conill','faiza','abestruz','zebra','ratpenat','cavall','ratoli']

    console.log(llistaAnimals)

    ```
2. fas una funció que retorni nivell (numero del 0-100) (Math.random)
    ```js
        function getRandomArbitrary(min, max)   
            {
                return Math.round(Math.random() * (max - min) + min);
            }

        getRandomArbitrary(0,100)

    ```


3. fas una funció que retorni 5 animals aleatoris diferents
    ```js
        function tornarValorsAleatoris(array, numvalors)   
            {
                let max = array.length  
                let min = 0
                let llistaValores=[]
                for(let i = 0; i <numvalors; ++i)
                    {
                        let valoraleatori = Math.round(Math.random() * (max - min) + min);
                        llistaValores.push(array[valoraleatori])
                        
                    }    
                return llistaValores;            
            }

        tornarValorsAleatoris(llistaAnimals,5)

    ```
4. fas una funció que retorni un usuari (objecte que té nivell (0-100, i té 5 animals (utilitzes la funció anterior)))
```js
    function tornarUsuari(numUser)   
            {
                let usuari = { 
                id: numUser,  
                nivell:getRandomArbitrary(0, 100) , 
                animal:[tornarValorsAleatoris(llistaAnimals, 5) ]}
  
                return usuari;            
            }

    tornarUsuari(1)
```



5. fas una funció que retorni una llista de 100 usuaris
```js
    function tornarUsuari(numUser)   
            {   
                let llistaUsuaris=[] 

                for(let i = 0; i <numUser; ++i)
                    {
                        let usuari = { 
                        id: i,  
                        nivell:getRandomArbitrary(0, 100) , 
                        animal:[tornarValorsAleatoris(llistaAnimals, 5) ]
                        }
                          
                        llistaUsuaris.push(usuari)
                        
                    }  

                
  
                return llistaUsuaris;            
            }

    tornarUsuari(100)    
```


---
6. fas una funció que retorni un objecte on les claus seràn els animals i els valors seràn els ids dels usuaris (els que els hi agrada aquell animal)
```js
{
    foca: [ 0, 1 ],
    elefant: [ 0 ],
    pantera: [ 0 ],
    tigre: [ 0 ],
    dofi: [1 ],
    gos: [1 ],
    zebra: [1 ],

}
```


```js
 function BuscarUsuarisAniaml(nomAnimal,numUser)   
            {   
                let llistaUsuaris=[tornarUsuari(numUser)]
                for(let i = 0; i <numUser; ++i)
                    {
                        llistaUsuaris[i]   
                        for(let a = 0; a <numUser; ++a)
                        {
                            llistaUsuaris[animl[a]]
                            animal[usuaris[i].animal[a]].push(usuaris[i].nomAnimal)    
                        

                        }
   
                        

                    }
  
                return llistaUsuaris;            
            }


function tornarLlistaAnimaUsuari(numUser)   
            {   
                let llistaUsuaris=[tornarUsuari(numUser)]
                llistaAnimals['llop','serp','tigre','coala','oreneta','gat','gos','girafa','elefan','rinoceront','cocodril','ximpanze','izart','conill','faiza','abestruz','zebra','ratpenat','cavall','ratoli']
                for(let i = 0; i <20; ++i){
                    let Animals = { 
                        nom: llistaAnimals[i],  
                        usuaris:[BuscarUsuarisAniaml(Animals.nom,numUser) ]
                        }
                    }
  
                return llistaUsuaris;            
            }

```