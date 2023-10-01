# tabla-y-atributo

1) Tabla "Material":
 
Atributos:

id (Clave primaria, tipo: int)

nombre (tipo: string)

cantidadDisponible (tipo: int)

precioUnitario (tipo: double)

2) Tabla "Producto":

Atributos:

id (Clave primaria, tipo: int)

nombre (tipo: string)

precio (tipo: double)

3) Tabla "Cliente":

Atributos:

id (Clave primaria, tipo: int)

nombre (tipo: string)

direccion (tipo: string)

4) Tabla "Proveedor":

Atributos:

id (Clave primaria, tipo: int)

nombre (tipo: string)

direccion (tipo: string)

5) Tabla "Orden":

Atributos:

id (Clave primaria, tipo: int)

fecha (tipo: Date)

cliente (Clave foránea referente a la tabla Cliente)

proveedor (Clave foránea referente a la tabla Proveedor)

productos (Colección de Productos; esto podría ser una relación many-to-many)

6) Tabla "Factura":

Atributos:

id (Clave primaria, tipo: int)

fecha (tipo: Date)

orden (Clave foránea referente a la tabla Orden)

total (tipo: double)
