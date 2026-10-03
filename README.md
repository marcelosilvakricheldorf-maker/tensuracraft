# TensuraCraft: Isekai Crossover (Minecraft 1.21.1 · NeoForge)

Mod de fans **no oficial** inspirado en *Tensei Shitara Slime Datta Ken*, con facciones, personajes,
jefes y habilidades de **Re:Zero, Overlord, Konosuba y Bleach**. Todos los textos del juego están en español.

> Las texturas incluidas son skins **genéricas por facción** (no retratos de los personajes).
> Puedes darle a cada personaje la skin que quieras sin recompilar (ver *Skins personalizadas*).

---

## 1. Cómo compilar e instalar

Requisitos: **Java 21 (JDK)**, Minecraft **1.21.1** con **NeoForge 21.1.x**.

```bash
# Windows
gradlew.bat build
# Linux / Mac
./gradlew build
```

El `.jar` queda en `build/libs/tensuracraft-1.0.0.jar` → cópialo a la carpeta `mods` de tu instancia NeoForge 1.21.1.

* Para probar directamente: `gradlew runClient`.
* **Sin instalar nada:** sube la carpeta a un repositorio de GitHub; el workflow incluido
  (`.github/workflows/build.yml`) compila el mod y deja el `.jar` en *Actions → Artifacts*.
* Si Gradle no encuentra la versión de NeoForge, cambia `neo_version` en `gradle.properties`
  por la última `21.1.x` publicada (y/o la versión del plugin `net.neoforged.moddev` en `build.gradle`).

---

## 2. Primeros pasos

1. Al entrar al mundo se abre la pantalla de **Reencarnación**: eliges tu raza inicial.
2. Naces con las habilidades innatas de tu raza **+ una "Bendición del reencarnado"** aleatoria
   (Extra, o Única con 30% de probabilidad).
3. Pulsa **K** para el menú de estado. Asigna habilidades a las ranuras **Z / X / C** y úsalas con esas teclas.
4. Busca ciudades, habla con los personajes (clic derecho) y acepta misiones.

| Tecla | Acción |
|---|---|
| K | Menú: Estado / Habilidades / Misiones / Facciones (o elegir raza si aún no tienes) |
| Z, X, C | Usar la habilidad de la ranura 1, 2, 3 |
| Shift + clic derecho a un monstruo/lobo | **Nombrarlo** (con una etiqueta renombrada usa ese nombre) |
| Shift + clic derecho a un subordinado | Quedarse quieto / seguirte |

---

## 3. Razas y líneas evolutivas (19 razas iniciales, 3 etapas cada una)

| Serie | id | Línea evolutiva |
|---|---|---|
| Tensura | `human` | Humano → Humano Iluminado → Santo |
| Tensura | `slime` | Slime → Slime Demoniaco (Senor Demonio) → Slime Dios Dragon |
| Tensura | `goblin` | Goblin → Hobgoblin → Rey Goblin |
| Tensura | `ogre` | Ogro → Kijin → Oni (Kishin) |
| Tensura | `orc` | Orco → Orco Superior → Desastre Orco |
| Tensura | `lizardman` | Hombre Lagarto |
| Tensura | `dwarf` | Enano → Enano Ancestral → Rey Heroe Enano |
| Tensura | `elf` | Elfo → Alto Elfo → Elfo Ancestral |
| Tensura/Overlord | `vampire` | Vampiro → Vampiro Verdadero → Progenitor Vampiro |
| Tensura | `lesser_demon` | Demonio Menor → Demonio Mayor → Archidemonio |
| Tensura | `dragonoid` | Dragonoide |
| Tensura/Re:Zero | `spirit` | Espiritu Menor |
| Re:Zero | `half_elf` | Medio Elfo → Medio Elfo Espiritista → Medio Elfo de Hielo Eterno |
| Re:Zero/Tensura | `beastman` | Hombre Bestia → Hombre Bestia Feroz → Rey Bestia |
| Overlord | `skeleton` | Esqueleto (No-Muerto) → Lich Anciano → Overlord |
| Konosuba | `crimson_demon` | Demonio Carmesi → Archimago Carmesi → Maestro de la Explosion |
| Bleach | `shinigami` | Shinigami → Teniente Shinigami (Shikai) → Capitan Shinigami (Bankai) |
| Bleach | `hollow` | Hollow → Adjuchas → Arrancar (Espada) |
| Bleach | `quincy` | Quincy → Sternritter → Quincy Vollstandig |

* Cada raza cambia vida, ataque, velocidad, armadura, **tamaño** (el Slime mide la mitad), magículas y regeneración.
* Rasgos: inmunidad al fuego, respirar bajo el agua, visión nocturna, sin daño por caída, no-muerto,
  regeneración, debilidad solar (vampiro), vuelo permanente, minero experto, agilidad, adaptable (+25% EP).
* **EP (Puntos de Existencia):** se ganan matando, devorando, con misiones y cristales. Suben tus magículas máximas,
  tu vida/ataque y el daño de tus habilidades (hasta x3).
* **Festival de la Cosecha:** algunas evoluciones (Señor Demonio, Verdadero Dragón, Overlord, Arrancar...) requieren
  **almas** (matar jugadores, aldeanos, NPCs humanoides y jefes, o usar Fragmentos de Alma). Otorgan un regalo Único
  y tus subordinados con nombre también se fortalecen.
* Evolucionas desde el menú K (botón *¡Evolucionar!*) o con `/tensura evolucionar`.

---

## 4. Habilidades (80) y Gacha

- **Común** (13): Resistencia al Calor (Tensura), Resistencia al Veneno (Tensura), Vision Oscura (Overlord), Hilo Pegajoso (Tensura), Cuchilla de Agua (Tensura), Aliento Venenoso (Tensura), Intimidacion (Tensura), Shamac (Re:Zero), Murak (Re:Zero), Tinder (Konosuba), Freeze (Konosuba), Hado #4: Byakurai (Bleach), Fura (Re:Zero)
- **Extra** (32): Percepcion Magica (Tensura), Regeneracion Ultrarrapida (Tensura), Cuerpo de Acero (Tensura), Aceleracion del Pensamiento (Tensura), Suerte Absurda (Konosuba), Hierro (Bleach), Blut Vene (Bleach), Hilo de Acero (Tensura), Aliento Paralizante (Tensura), Rayo Negro (Tensura), Llama Negra (Tensura), Movimiento Sombra (Tensura), Mimetismo (Tensura), Alas Magicas (Tensura), Fly (Overlord), Corte Instantaneo (Tensura), Llamado de la Manada (Tensura), Al Huma (Re:Zero), El Goa (Re:Zero), Invocar Espiritu de Hielo (Re:Zero), Robar (Steal) (Konosuba), Purificacion Sagrada (Konosuba/Tensura), Sanacion Sagrada (Konosuba/Tensura), Provocar (Decoy) (Konosuba), Drain Touch (Konosuba), Light of Saber (Konosuba), Shunpo / Sonido (Bleach), Cero (Bleach), Hado #33: Sokatsui (Bleach), Bakudo #61: Rikujokoro (Bleach), Heilig Pfeil (Bleach), Presion Espiritual (Bleach)
- **Única** (24): Gran Sabio (Tensura), Glotoneria (Tensura), Cocinero (Tensura), Regreso por Muerte (Re:Zero), Aura de Desesperacion (Overlord), Depredador (Tensura), Invocar Ifrit (Tensura), Haki del Rey Demonio (Tensura), Llamarada Infernal (Hell Flare) (Tensura), Replicacion (Tensura), Tentador (Tensura), Desintegracion (Tensura), Mano Invisible (Pereza) (Re:Zero), Agarrar Corazon (Overlord), Crear No-Muerto (Overlord), ¡Explosion! (Konosuba), Maldicion de Muerte (Konosuba), Getsuga Tensho (Bleach), Bankai (Bleach), Gran Rey Cero (Bleach), Resurreccion / Mascara Hollow (Bleach), Senbonzakura Kageyoshi (Bleach), Primera Danza: Tsukishiro (Bleach), Lanza del Relampago (Bleach)
- **Definitiva** (11): Rafael, Senor de la Sabiduria (Tensura), Bendicion del Santo de la Espada (Re:Zero), Belcebu, Senor de la Glotoneria (Tensura), Dragon de la Tormenta (Veldora) (Tensura), Drago Nova (Tensura), Corazon de Leon (Codicia) (Re:Zero), Detener el Tiempo (Overlord), Corte de la Realidad (Overlord), Fallen Down (Overlord), Kyoka Suigetsu (Hipnosis Completa) (Bleach), Hado #90: Kurohitsugi (Bleach)

* **Gacha del Destino:** usa un *Orbe del Destino* (clic derecho). Probabilidades base: Común 55% · Extra 30% ·
  Única 12% · Definitiva 3%. Sistema de **pity**: Única garantizada cada 30 tiradas (configurable).
  *Suerte Absurda* y la raza Humana mejoran las probabilidades.
* **Depredador / Belcebú:** devora a un enemigo debilitado (<50% / <70% de vida): ganas EP y puedes **copiar** una
  habilidad según la criatura (araña → Hilo, blaze → Llama Negra, enderman → Movimiento Sombra, NPC → una de sus habilidades...).
* **Gran Sabio / Rafael:** analizan lo que miras y reducen enfriamientos y coste de MP.
* **Regreso por Muerte:** al morir vuelves a tu último punto de control (se guarda cada 2 min).
* **Grimorios:** enseñan una habilidad concreta (los sueltan jefes y dragones).

---

## 5. Nombramientos e invocaciones

* **Nombrar** cuesta magículas según la fuerza del ser. Si no te alcanzan caes en *Modo de Baja Magícula*.
  Goblin → Hobgoblin, Ogro → Kijin, Hombre Lagarto → Dragonewt, Orco → Orco Superior, Lobo → **Lobo Tempestad**.
  El ser nombrado se vuelve tu subordinado leal, te sigue, pelea por ti y lleva tu apellido.
* **Invocaciones:** Ifrit, Clones de Sombra, Espíritu de Hielo, Caballeros de la Muerte, Lobos Tempestad, Ángeles (Slane).
* Si consigues **Depredador** y hablas con **Veldora** en su cueva, te dará su poder y el apellido **Tempest**.

---

## 6. Facciones, NPCs, jefes y dragones (92 tipos de NPC)

Facciones: Tempest, Dwargon, Blumund, Iglesia Sagrada, Señores Demonio, Horda Orca, Lugunica, Culto de la Bruja,
Nazarick, Re-Estize, Teocracia de Slane, Gremio de Axel, Ejército del Rey Demonio, Gotei 13, Hueco Mundo y Monstruos.

* Tu **reputación** (−1000 a 1000) decide quién te ataca. ≥50 = aliado, ≤−50 = hostil. Tu raza empieza con +100 en su facción.
* Las facciones se pelean entre sí (los guardias de las ciudades defienden de monstruos y de facciones enemigas).
* La **Iglesia Sagrada** y la **Teocracia de Slane** atacan a razas no humanas.
* Si atacas a un NPC pacífico, sus aliados cercanos acuden a defenderlo.
* **Jefes** con barra de vida, fase 2 al 50% y botín (orbes, grimorios): Geld, Clayman, Milim, Ifrit (Shizu se
  transforma), Hinata, Petelgeuse, Regulus (*Corazón de León*: solo es vulnerable a intervalos), Elsa, Shalltear, Nigun,
  Beldia, Hans, Vanir, Kenpachi, Grimmjow, Ulquiorra y Aizen.
* **Dragones** voladores: Veldora, Velgrynd, Velzard, Volcanica (neutrales hasta que los provocas), Dragón de Escarcha y Wyvern.

| id (para skins) | Nombre | Serie | Facción | Rol |
|---|---|---|---|---|
| `goblin` | Goblin | Tensura | TEMPEST | CIVILIAN |
| `hobgoblin` | Hobgoblin | Tensura | TEMPEST | GUARD |
| `rigurd` | Rigurd | Tensura | TEMPEST | QUEST_GIVER |
| `gobta` | Gobta | Tensura | TEMPEST | GUARD |
| `rimuru` | Rimuru Tempest | Tensura | TEMPEST | QUEST_GIVER |
| `benimaru` | Benimaru | Tensura | TEMPEST | GUARD |
| `shuna` | Shuna | Tensura | TEMPEST | CIVILIAN |
| `shion` | Shion | Tensura | TEMPEST | GUARD |
| `souei` | Souei | Tensura | TEMPEST | GUARD |
| `hakurou` | Hakurou | Tensura | TEMPEST | GUARD |
| `diablo` | Diablo | Tensura | TEMPEST | GUARD |
| `gabiru` | Gabiru | Tensura | TEMPEST | GUARD |
| `ogre` | Ogro | Tensura | MONSTERS | GUARD |
| `kijin` | Kijin | Tensura | TEMPEST | GUARD |
| `lizardman` | Hombre Lagarto | Tensura | TEMPEST | GUARD |
| `dragonewt` | Dragonewt | Tensura | TEMPEST | GUARD |
| `high_orc` | Orco Superior | Tensura | TEMPEST | GUARD |
| `shadow_clone` | Clon de Sombra | Tensura | TEMPEST | SUMMON |
| `treyni` | Treyni (Driade) | Tensura | TEMPEST | CIVILIAN |
| `orc` | Orco | Tensura | ORC_HORDE | ENEMY |
| `geld` | Geld, el Desastre Orco | Tensura | ORC_HORDE | BOSS |
| `lesser_demon` | Demonio Menor | Tensura | DEMON_LORDS | ENEMY |
| `clayman` | Clayman | Tensura | DEMON_LORDS | BOSS |
| `milim` | Milim Nava | Tensura | DEMON_LORDS | BOSS |
| `ifrit` | Ifrit | Tensura | MONSTERS | BOSS |
| `ifrit_summon` | Ifrit (Invocado) | Tensura | TEMPEST | SUMMON |
| `dwarf` | Enano | Tensura | DWARGON | CIVILIAN |
| `dwarf_guard` | Guardia Enano | Tensura | DWARGON | GUARD |
| `kaijin` | Kaijin | Tensura | DWARGON | QUEST_GIVER |
| `gazel` | Gazel Dwargo | Tensura | DWARGON | GUARD |
| `blumund_villager` | Ciudadano de Blumund | Tensura | BLUMUND | CIVILIAN |
| `adventurer` | Aventurero | Tensura | BLUMUND | GUARD |
| `fuze` | Fuze | Tensura | BLUMUND | QUEST_GIVER |
| `shizu` | Shizu | Tensura | BLUMUND | GUARD |
| `holy_knight` | Caballero Sagrado | Tensura | HOLY_CHURCH | GUARD |
| `hinata` | Hinata Sakaguchi | Tensura | HOLY_CHURCH | BOSS |
| `emilia` | Emilia | Re:Zero | LUGUNICA | GUARD |
| `subaru` | Natsuki Subaru | Re:Zero | LUGUNICA | QUEST_GIVER |
| `rem` | Rem | Re:Zero | LUGUNICA | GUARD |
| `ram` | Ram | Re:Zero | LUGUNICA | GUARD |
| `beatrice` | Beatrice | Re:Zero | LUGUNICA | CIVILIAN |
| `roswaal` | Roswaal L. Mathers | Re:Zero | LUGUNICA | QUEST_GIVER |
| `reinhard` | Reinhard van Astrea | Re:Zero | LUGUNICA | GUARD |
| `lugunica_knight` | Caballero de Lugunica | Re:Zero | LUGUNICA | GUARD |
| `ice_spirit` | Espiritu de Hielo | Re:Zero | LUGUNICA | SUMMON |
| `cultist` | Adepto del Culto de la Bruja | Re:Zero | WITCH_CULT | ENEMY |
| `petelgeuse` | Petelgeuse Romanee-Conti | Re:Zero | WITCH_CULT | BOSS |
| `regulus` | Regulus Corneas | Re:Zero | WITCH_CULT | BOSS |
| `elsa` | Elsa Granhiert | Re:Zero | MONSTERS | BOSS |
| `ainz` | Ainz Ooal Gown | Overlord | NAZARICK | QUEST_GIVER |
| `albedo` | Albedo | Overlord | NAZARICK | GUARD |
| `shalltear` | Shalltear Bloodfallen | Overlord | NAZARICK | BOSS |
| `demiurge` | Demiurge | Overlord | NAZARICK | GUARD |
| `cocytus` | Cocytus | Overlord | NAZARICK | GUARD |
| `aura` | Aura Bella Fiora | Overlord | NAZARICK | GUARD |
| `mare` | Mare Bello Fiore | Overlord | NAZARICK | GUARD |
| `sebas` | Sebas Tian | Overlord | NAZARICK | GUARD |
| `death_knight` | Caballero de la Muerte | Overlord | NAZARICK | GUARD |
| `skeleton_warrior` | Guerrero Esqueleto | Overlord | NAZARICK | ENEMY |
| `elder_lich_npc` | Lich Anciano | Overlord | NAZARICK | ENEMY |
| `gazef` | Gazef Stronoff | Overlord | RE_ESTIZE | QUEST_GIVER |
| `re_estize_soldier` | Soldado de Re-Estize | Overlord | RE_ESTIZE | GUARD |
| `sunlight_priest` | Sacerdote de la Escritura Solar | Overlord | SLANE | ENEMY |
| `nigun` | Nigun Grid Luin | Overlord | SLANE | BOSS |
| `angel` | Angel Arcangel de la Llama | Overlord | SLANE | SUMMON |
| `kazuma` | Satou Kazuma | Konosuba | AXEL | QUEST_GIVER |
| `aqua` | Aqua | Konosuba | AXEL | CIVILIAN |
| `megumin` | Megumin | Konosuba | AXEL | GUARD |
| `darkness` | Darkness | Konosuba | AXEL | GUARD |
| `wiz` | Wiz | Konosuba | AXEL | CIVILIAN |
| `vanir` | Vanir | Konosuba | DEVIL_KING | BOSS |
| `yunyun` | Yunyun | Konosuba | AXEL | GUARD |
| `luna` | Luna (Recepcionista) | Konosuba | AXEL | QUEST_GIVER |
| `axel_adventurer` | Aventurero de Axel | Konosuba | AXEL | GUARD |
| `devil_king_soldier` | Soldado del Rey Demonio | Konosuba | DEVIL_KING | ENEMY |
| `beldia` | Beldia, el Caballero Sin Cabeza | Konosuba | DEVIL_KING | BOSS |
| `hans` | Hans, el Slime Venenoso | Konosuba | DEVIL_KING | BOSS |
| `ichigo` | Kurosaki Ichigo | Bleach | GOTEI_13 | GUARD |
| `rukia` | Kuchiki Rukia | Bleach | GOTEI_13 | GUARD |
| `renji` | Abarai Renji | Bleach | GOTEI_13 | GUARD |
| `byakuya` | Kuchiki Byakuya | Bleach | GOTEI_13 | GUARD |
| `kenpachi` | Zaraki Kenpachi | Bleach | GOTEI_13 | BOSS |
| `urahara` | Urahara Kisuke | Bleach | GOTEI_13 | QUEST_GIVER |
| `yamamoto` | Yamamoto Genryusai | Bleach | GOTEI_13 | GUARD |
| `uryu` | Ishida Uryu | Bleach | GOTEI_13 | GUARD |
| `shinigami` | Shinigami | Bleach | GOTEI_13 | GUARD |
| `hollow` | Hollow | Bleach | HUECO_MUNDO | ENEMY |
| `menos` | Menos Grande | Bleach | HUECO_MUNDO | ENEMY |
| `arrancar` | Arrancar | Bleach | HUECO_MUNDO | ENEMY |
| `grimmjow` | Grimmjow Jaegerjaquez | Bleach | HUECO_MUNDO | BOSS |
| `ulquiorra` | Ulquiorra Cifer | Bleach | HUECO_MUNDO | BOSS |
| `aizen` | Sosuke Aizen | Bleach | HUECO_MUNDO | BOSS |

---

## 7. Ciudades y estructuras (generación natural)

| Estructura | Bioma | Contenido |
|---|---|---|
| Tempest | bosque, llanura | Rimuru, Rigurd (misiones), Benimaru, Shuna, Shion, Souei, Hakurou, Diablo, goblins... |
| Reino de Dwargon | colinas, pradera | Salón real con Gazel, Kaijin (misiones), forjas enanas |
| Blumund | llanura, pradera | Ciudad humana, gremio de Fuze (misiones), Shizu |
| Catedral Sagrada | llanura, cerezos | Hinata y caballeros sagrados |
| Campamento Orco | pantano, sabana, taiga | Geld y la horda |
| Capital de Lugunica | llanura | Subaru y Roswaal (misiones), Emilia, Rem, Ram, Beatrice, Reinhard |
| Escondite del Culto | bosque oscuro, taiga | Petelgeuse, Regulus y cultistas |
| Gran Tumba de Nazarick | llanura, sabana, badlands | Ainz (misiones), guardianes, cripta de Shalltear |
| Puesto de Re-Estize | llanura, sabana | Gazef (misiones) |
| Axel | llanura, pradera | Gremio (Luna), Kazuma, Aqua, Megumin, Darkness, tienda de Wiz con Vanir |
| Castillo de Beldia | llanura, bosque | Beldia y soldados del Rey Demonio |
| Seireitei | cerezos, llanura | Urahara (misiones), Ichigo, Rukia, Renji, Byakuya, Kenpachi, Yamamoto |
| Las Noches | desierto | Aizen, Ulquiorra, Grimmjow, arrancars |
| Cueva de Veldora | taiga | Veldora sellado |
| Salón de Walpurgis | badlands | Milim y Clayman |
| Nido de Escarcha | llanuras nevadas | Dragón de Escarcha |

Además aparecen enemigos salvajes de noche/en cuevas: orcos, demonios menores, cultistas, guerreros esqueleto,
liches, sacerdotes de Slane, soldados del Rey Demonio, hollows, arrancars y Menos Grande (también en el Nether).

**Misiones:** 36 misiones en cadenas por personaje (matar, recolectar, nombrar, evolucionar, conseguir habilidad).

---

## 8. Objetos y recetas

| Objeto | Uso | Receta |
|---|---|---|
| Orbe del Destino | Tirada de gacha | Oro + amatista + diamante (o 8 Fragmentos de Alma + diamante) |
| Cristal de Magículas | +150 MP, +40 EP | Lapislázuli + amatista + cuarzo |
| Fragmento de Alma | +1 alma | Botín |
| Elixir de Reencarnación | Cambiar de raza | Tótem + Orbe + botella + lágrima de ghast |
| Katana de Tempest | Espada de netherita mejorada | Escama de dragón + diamante + palo |
| Zanpakutō | Shikai (clic der.), Getsuga (Shift) | Diamante + Fragmento de Alma + palo |
| Bastón Carmesí | Bola de fuego / ¡Explosión! (Shift) | Cristal de Magículas + 2 varas de blaze |
| Grimorio / Pergamino de Invocación / Sello de Dragón | Habilidad / NPC / Dragón | Botín o creativo |

---

## 9. Comandos

* `/tensura raza` · `/tensura raza lista` · `/tensura estado` · `/tensura evolucionar`
* `/tensura habilidades` · `/tensura misiones` · `/tensura facciones`
* `/tensura mision aceptar <id>` · `/tensura mision abandonar <id>`
* Admin (op): `/tensura admin habilidad|raza|ep|almas|gacha|reiniciar <jugador> ...`

Configuración en `config/tensuracraft-common.toml`: destrucción de bloques de habilidades, daño entre jugadores,
multiplicadores de MP y EP, pity del gacha y enfriamiento de Regreso por Muerte.

---

## 10. Skins personalizadas (sin recompilar)

Crea un *resource pack* con esta ruta y coloca skins de Minecraft normales (64×64):

```
assets/tensuracraft/textures/entity/npc/<id>.png      ej.: rimuru.png, emilia.png, ainz.png, ichigo.png
assets/tensuracraft/textures/entity/dragon/<id>.png   veldora, velgrynd, velzard, volcanica, frost_dragon, wyvern (128×128)
```

Si existe un archivo con el id del personaje, se usa; si no, se usa la skin genérica de su facción.

---

## 11. Estructura del código

```
src/main/java/com/marcelo/tensuracraft/
  race/      Razas, evolución, atributos            skill/   Habilidades, gacha, uso de MP
  npc/       Tipos de NPC y nombramientos           entity/  NPC humanoide y dragón
  quest/     Misiones                               faction/ Facciones y relaciones
  network/   Paquetes cliente-servidor              event/   Eventos del juego
  client/    Pantallas, HUD, teclas, render         item/    Objetos
src/main/resources/data/tensuracraft/  estructuras (.nbt), worldgen, recetas, spawns
```

Añadir contenido es sencillo: una raza = una línea en `Races.java`, un NPC = una línea en `NpcTypes.java`,
una misión = una línea en `Quests.java`, una habilidad = un bloque en `Skills.java`.

---
*Proyecto de fans sin fines de lucro. Tensura, Re:Zero, Overlord, Konosuba y Bleach pertenecen a sus respectivos autores.*
