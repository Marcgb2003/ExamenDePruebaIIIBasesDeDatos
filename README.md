# ExamenDePruebaIIIBasesDeDatos
1: Select * from piezas where color like 'rojo';
\
![image](https://github.com/Marcgb2003/ExamenDePruebaIIIBasesDeDatos/assets/122601138/993a211b-a3d2-4f19-ae84-161fc5e7c6d3)
\
2: Select * from proveedores where ciudad_proveedor like 'Madrid';
\
![image](https://github.com/Marcgb2003/ExamenDePruebaIIIBasesDeDatos/assets/122601138/645ee07d-b7ec-48d5-bb00-780cc2918fe5)
\
3: Select nombre_pieza from Piezas order by peso desc limit 1;
\
![image](https://github.com/Marcgb2003/ExamenDePruebaIIIBasesDeDatos/assets/122601138/be2bdbac-31ce-4d98-b5db-819c7f691a6b)
\
4:Select pro.nombre_proveedor from Proveedores pro inner join Piezas pi on pro.id_proveedor=pi.id_proveedor group by pro.nombre_proveedor order by count(pi.id_pieza) desc limit 1;
\
![image](https://github.com/Marcgb2003/ExamenDePruebaIIIBasesDeDatos/assets/122601138/f5bec1e7-18f3-4c60-8c89-a451e528b8cf)
\
5: Select pro.nombre_proveedor from Proveedores pro inner join Piezas pi on pro.id_proveedor=pi.id_proveedor where pi.color = 'azul';
\
![image](https://github.com/Marcgb2003/ExamenDePruebaIIIBasesDeDatos/assets/122601138/40358e68-4996-4b6b-a474-b96d319e4ecc)
\
6: Select nombre_pieza from piezas where id_proveedor in (select id_proveedor from proveedores where nombre_proveedor like 'Proveedor A') order by peso Limit 1;
\
![image](https://github.com/Marcgb2003/ExamenDePruebaIIIBasesDeDatos/assets/122601138/663f41ef-c0da-4d48-a799-7cf0b139f0f6)
\
7: Select nombre_proveedor from proveedores where id_proveedor = (Select id_proveedor from piezas order by peso limit 1);
\
![image](https://github.com/Marcgb2003/ExamenDePruebaIIIBasesDeDatos/assets/122601138/c73589f5-2877-4829-bc5b-d6543f12c065)
\
8: Select * from Piezas where id_proveedor in (select id_proveedor from proveedores where ciudad_proveedor like 'Barcelona');
\
![image](https://github.com/Marcgb2003/ExamenDePruebaIIIBasesDeDatos/assets/122601138/2c8c7e54-ffde-450f-91d1-45c2d46f4cb3)
\
9:Select pr.nombre_proveedor from Proveedores pr inner join Piezas pi on pr.id_proveedor=pi.id_proveedor where pi.color like 'verde' group by pr.nombre_proveedor order by count(id_pieza) desc limit 1;
\
![image](https://github.com/Marcgb2003/ExamenDePruebaIIIBasesDeDatos/assets/122601138/b6f198f1-e26d-423f-9dab-cebf93eb9dc1)
\
10: select nombre_pieza from piezas where id_proveedor in (select id_proveedor from proveedores where ciudad_proveedor like 'Valencia') order by peso desc limit 1;
\
![image](https://github.com/Marcgb2003/ExamenDePruebaIIIBasesDeDatos/assets/122601138/af2c3914-5556-45b1-a29d-b2dd00a85e10)
