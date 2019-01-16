> # IMEX-API
  
  
### Wzory zapytań

GET Header

* Lista kierowcówców **{drivers}**, zamówień **{orders}**, ciężarówek **{trucks}**.  
`https://example.com/{drivers/orders/trucks}`  

* Lista zależna od informacji z działaniami na zbiorach **{equal-to}**, **{in}**, **{smaller-than}**, **{bigger-than}**.  
`https://example.com/{drivers/orders/trucks}/that-have-{własność}-{działanie}-{wartość}`

* Lista zależna od kilku informacji ze wzorca powyżej połączonymi słowami wykluczających **and** lub sumujących **or**.  
`https://example.com/{drivers/orders/trucks}/that-have-{informacja}-{and/or}-{informacja}`

* Pierwszy kierowca **{driver}**, zamówienie **{order}**, ciężarówka **{truck}** odnalezione po informacji.  
`https://example.com/{driver/order/truck}/that-have-{własność}-{equal-to/in/smaller-than/bigger-than}-{wartość}`

* Pierwszy odnaleziony po kilku informacjach.  
`https://example.com/{driver/order/truck}/that-have-{that-have}-{and/or}-{that-have}`
