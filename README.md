# Olá, Mundo!
## Esse é um arquivo de Estudo
---
[Acesse o código](https://code.earthengine.google.com/)
### Estudos do João Victor

**Primeiro** Repositório Versionado 🖖

__Repositório__ Teste para *GitHub*
* Serve para __*itálico*__

Essa ~~Linha~~ eu fiz no site!

Lista numerada

1. test
   1. test

 Lista demarcada
 * Test
    * Test

Lista de Tarefas

- [X] Criar algo
- [ ] Blablabla

num | aluno | nota
---|---|---
1 | gust | 9.3
2 | alune | 505

Não estou conseguindo usar o `var img = ee.image.Collection('Copernicus_16165165_ST_SR')`

```
// Here, you use the limit() function to keep the most recent image, by taking the first
// image from a list of images, sorted by the time_start variable
var firstimg=dataset.limit(1, 'system:time_start', true);
var lastimg=dataset.limit(1, 'system:time_start', false);
var diffimg=firstimg.subtract(lastimg);
var seaSurfaceTemperature = diffimg.select('sst');
var visParams = {
  min: -180.0,
  max: 3000.0,
  palette: [
    '040274', '040281', '0502a3', '0502b8', '0502ce', '0502e6',
    '0602ff', '235cb1', '307ef3', '269db1', '30c8e2', '32d3ef',
    '3be285', '3ff38f', '86e26f', '3ae237', 'b5e22e', 'd6e21f',
    'fff705', 'ffd611', 'ffb613', 'ff8b13', 'ff6e08', 'ff500d',
    'ff0000', 'de0101', 'c21301', 'a71001', '911003'
  ],
};
Map.setCenter(20.3, -20.39, 2);
Map.addLayer(seaSurfaceTemperature, visParams, 'Sea Surface Temperature');
```



