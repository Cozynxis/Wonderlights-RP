# Blockbench-modellen toevoegen

1. Maak of open je model in Blockbench.
2. Exporteer als Java Block/Item model.
3. Zet de JSON in `assets/wonderlights/models/item/`.
4. Zet de normale PNG in `assets/wonderlights/textures/item/`.
5. Maak daarnaast een emissive PNG met dezelfde afmetingen en voeg `_e` aan de naam toe.

Voorbeeld:

```text
attractielamp.json
attractielamp.png
attractielamp_e.png
```

Gebruik in het model bijvoorbeeld:

```json
"textures": {
  "0": "wonderlights:item/attractielamp"
}
```

In de `_e.png` maak je alles transparant behalve de pixels die in het donker helder moeten blijven.

## Belangrijk

Emissive pixels blijven helder zichtbaar, maar verlichten de omgeving niet automatisch met gekleurd licht. Voor gekleurde lichtprojectie op muren/vloeren heb je daarnaast een geschikte shader/mod-renderingoplossing nodig.
