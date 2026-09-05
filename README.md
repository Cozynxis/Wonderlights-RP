# Wonderlights-RP

Minecraft Java 1.21.10 resource pack voor custom Blockbench-modellen en emissive/colored-lighting effecten.

## Doel

- Custom 3D modellen uit Blockbench
- Emissive textures die zichtbaar blijven in het donker
- Geschikt om via GitHub te beheren en te versioneren
- Basis voor lampen, spots, neon, attracties, borden, gebouwen en decoratie

## Emissive textures

Voor een gewone texture:

`assets/wonderlights/textures/item/example_lamp.png`

maak je een tweede texture:

`assets/wonderlights/textures/item/example_lamp_e.png`

De `_e` texture bevat alleen de delen die moeten gloeien. Niet-gloeiende delen maak je transparant.

De instelling staat in:

`assets/minecraft/optifine/emissive.properties`

met:

```properties
suffix.emissive=_e
```

> Emissive textures laten het model zelf helder lijken in het donker. Ze geven zonder extra shader/mod geen echt gekleurd licht af op omliggende blokken.

## Structuur

```text
assets/
├─ minecraft/
│  └─ optifine/
│     └─ emissive.properties
└─ wonderlights/
   ├─ models/
   │  └─ item/
   └─ textures/
      └─ item/
```

## Blockbench

Exporteer je model als Java Block/Item model en gebruik bij voorkeur de namespace `wonderlights`.
