# Gastronomicon Drake

Addon culinario de Slimefun mantenido por DrakesCraft Labs. Añade cadenas de
ingredientes, comidas, bebidas, fermentación, pesca y cultivos sin reemplazar
los ítems ni las recetas ya existentes en un mundo.

## Compatibilidad

- Paper o Purpur `1.21.11`
- Java `21`
- Slimefun Core Drake `11.0-Drake-1.21.1-SNAPSHOT`

Las integraciones con ExoticGarden, DynaTech y SlimeHUD son opcionales. Se
detectan al iniciar y pueden desactivarse desde `config.yml` cuando corresponda.

## Mantenimiento Drake

La rama principal compila contra el API moderno de Paper: los biomas se resuelven
por `NamespacedKey` y los objetos de pócima usan `PotionMeta#setBasePotionType`.
Esto conserva las familias climáticas, recetas, IDs y datos legacy de las
instalaciones existentes.

## Desarrollo

```bash
mvn -B -ntp clean verify
```

El artefacto generado queda en `target/Gastronomicon-drake v*.jar`. Antes de
reemplazar un JAR de producción, valida en staging una receta existente, un
fermentador y una trampa de cangrejos.

## Créditos

Proyecto original de SchnTgaiSpock. Algunas texturas de cabezas provienen o se
derivan de [minecraft-heads.com](https://minecraft-heads.com/).
