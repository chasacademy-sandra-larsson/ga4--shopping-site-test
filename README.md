# Javascipt Shopping Site

## Syfte: Öva arraymetoder, template literals, array destructering i ett samman hang.

## Dummy data: Vi använder oss av Fake Store API (https://fakestoreapi.com/) och använder oss av anropet 
 
 fetch('https://fakestoreapi.com/products')
            .then(res=>res.json())
            .then(json=>console.log(json))
            
   Output: 
   
            //output
            [
                {
                    id:1,
                    title:'...',
                    price:'...',
                    category:'...',
                    description:'...',
                    image:'...'
                },
                /*...*/
                {
                    id:30,
                    title:'...',
                    price:'...',
                    category:'...',
                    description:'...',
                    image:'...'
                }
            ]
            
För att spara användarens "shopping cart" använder vi oss av LocalStorage.

Startkoden innehåller hämtning av data (asynkron) och hämtning av data från LocalStorage samt skellet till de funktioner som kan användas så att shoppen
- Generera dynamisk html för alla produkter från hämtningen av fetch('https://fakestoreapi.com/products')
- Användaren kan lägga till en produkt i "basket"
- Användaren kan ta bort en produkt från "basket"
- Summan av alla produkter (i antal) ska visas vid kundvagnsikonen


### 1. Generera dynamisk html för alla produkten

Använd Array.prototype.map för att generera html-markup för varje product från förfrågan

    <div id=product-id-??? class="item">
            <img width="220" src=??? url alt=""> 
            <div class="details">
                <h3>???</h3>
                <p>???</p>
                <div class="price-quantity">
                <h2>$ ??? </h2>
                <div class="buttons">
                    <i onclick="decrement(???)" class="bi bi-dash-lg"></i>
                    <div id=??? class="quantity">
                    </div>
                    <div id=??? class="quantity">???</div>
                    <i onclick="increment(???)" class="bi bi-plus-lg"></i>
                </div>
                </div>
            </div>
        </div>
# ga4--shopping-site-test
# ga4--shopping-site-test
